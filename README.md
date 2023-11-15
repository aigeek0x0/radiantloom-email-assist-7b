<img src="https://huggingface.co/aigeek0x0/radiantloom-email-assist-7b/resolve/main/Radiantloom_Email_Assist.png" alt="Radiantloom Email Assist" width="800" style="margin-left:'auto' margin-right:'auto' display:'block'"/>

## Radiantloom Email Assist 7B
[Radiantloom Email Assist 7B](https://huggingface.co/aigeek0x0/radiantloom-email-assist-7b) is an email-assistant large language model fine-tuned from [Zephyr-7B-Beta](https://huggingface.co/HuggingFaceH4/zephyr-7b-beta), over a custom-curated dataset of 1,000 email-assistant summarization tasks prepared by AI Geek Labs. The context lenght for the model is 4096 and it is licensed for commercial use.

## Intended Uses & Limitations
radiantloom-email-assist-7b is fine-tuned specifically for summarizing personal and business emails, converting them into voice memos, or chat messages.

It is not a state-of-the-art generative language model and is not designed to perform competitively on general tasks with more modern model architectures or models subject to larger pretraining corpuses.

## Prompt Template

```
<s>[INST]
<<SYS>>Given an input, provide a clear and concise summary and action items in less than 50 words.<</SYS>>
Answer the question below from context below :
Convert the summary into a voice memo, keeping it under one minute.
{{email_text}}
[/INST]</s>
```


## Model Usage
We encourage you to try out this model using Google Colab.
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Lvt30_gm2_4D-XSBNkX1k45j79fnNJtv#scrollTo=Wa2WjDcOxb8h)

Here are a few example use cases. if we query the model with

```
<s>[INST]
<<SYS>>Given an input, provide a clear and concise summary and action items in less than 50 words.<</SYS>>
Answer the question below from context below :

Convert the summary into a voice memo, keeping it under one minute.

From: deb@example.com
To: tan@xyz.com
Subject: Review and Feedback on Radiantloom Models for Business Integration

Hi Tan,

I hope this email finds you well. We are currently in the process of exploring Radiantloom models for potential integration into our business operations. Specifically, we are interested in your insights on the "radiantloom-email-assist-7b" model.

To ensure that we make well-informed decisions, we kindly request that you take some time to thoroughly review the documentation provided for this particular model. Your expertise and perspective are valuable to us, and we would appreciate any insights or observations you can share regarding the features, capabilities, and potential benefits of the "radiantloom-email-assist-7b" model.

If you come across any noteworthy points, concerns, or suggestions during your review, please don't hesitate to bring them to our attention. Your feedback will play a crucial role in shaping our decision-making process as we assess the suitability of Radiantloom models for our business needs.

Thank you in advance for your time and effort in this matter. We look forward to hearing your thoughts and recommendations.

Best regards,

Deb
[/INST]</s>

```

the model will return

```
<</ASSISTANT>
You have an email from Deb about reviewing the "radiantloom-email-assist-7b" model for business integration. They're seeking your expert opinion on its features, capabilities, and benefits. Please provide feedback if you notice anything noteworthy during your review. This is important for our decision-making process. Thanks in advance.

Action Items:
1. Review the "radiantloom-email-assist-7b" model documentation.
2. Share any insights, concerns, or suggestions with Deb.
3. Respond to Deb with your feedback by the deadline.

```

and if we query the model with

```
<s>[INST]
<<SYS>>Given an input, provide a clear and concise summary and action items in less than 50 words.<</SYS>>

Answer the question below from context below :

Convert the summary into a chat message.

From: deb@example.com
To: tan@xyz.com
Subject: Review and Feedback on Radiantloom Models for Business Integration

Hi Tan,

I hope this email finds you well. We are currently in the process of exploring Radiantloom models for potential integration into our business operations. Specifically, we are interested in your insights on the "radiantloom-email-assist-7b" model.

To ensure that we make well-informed decisions, we kindly request that you take some time to thoroughly review the documentation provided for this particular model. Your expertise and perspective are valuable to us, and we would appreciate any insights or observations you can share regarding the features, capabilities, and potential benefits of the "radiantloom-email-assist-7b" model.

If you come across any noteworthy points, concerns, or suggestions during your review, please don't hesitate to bring them to our attention. Your feedback will play a crucial role in shaping our decision-making process as we assess the suitability of Radiantloom models for our business needs.

Thank you in advance for your time and effort in this matter. We look forward to hearing your thoughts and recommendations.

Best regards,

Deb


[/INST]</s>

```

the model will return

```
Tan, Deb from example.com is seeking your feedback on the "radiantloom-email-assist-7b" model for business integration. Please review the related documents and share any insights, comments, or suggestions by reply. Thanks in advance!
Action Items:
1. Review the "radiantloom-email-assist-7b" model documentation.
2. Provide feedback and insights to Deb via email.
3. Respond within a reasonable timeframe.

```

## Evaluations
We are encouraged by the initial assessments conducted using the [LLM-as-a-Judge method](https://arxiv.org/abs/2306.05685), particularly with the utilization of GPT-4. Our ongoing efforts involve a more comprehensive evaluation of the model. As we progress, we will continue to provide updates on our findings and share the results on this platform.

## About Radiantloom
Radiantloom trains open-source large language models tailored for specific business tasks such as email assistance, customer support, and database operations.

Leran more about Radiantloom by visiting our [website](https://radiantloom.com). Follow us on Twitter at [Radiantloom](https://twitter.com/radiantloom) to gain early access to upcoming Radiantloom large language models.
