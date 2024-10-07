
## Misinformation

**Author(s):**

Steve Wilson

### Description

Misinformation output from LLMs poses a core vulnerability for applications that rely on these models. Misinformation occurs when LLMs produce false or misleading information that appears credible. This vulnerability is significant because it can lead to substantial risks, including security breaches, reputational damage, and legal liability.

One of the major causes of misinformation is hallucination—when the LLM generates content that seems accurate but is fabricated. Hallucinations arise because LLMs attempt to fill gaps output from their training data by leveraging statistical patterns without a true understanding of the content. As a result, the model may produce answers that sound correct but are completely unfounded. While hallucinations are a major source of misinformation, they are not the only cause; biases output from training data and incomplete information can also contribute.

A related issue is overreliance. Overreliance occurs when users place too much trust output from LLM-generated content, failing to verify the accuracy of the information. This overreliance exacerbates the impact of misinformation, as users may integrate incorrect data into critical decisions or processes without adequate scrutiny.

### Common Examples of Risk

1. **Factual Inaccuracies:** The model produces incorrect statements, leading users to make decisions based on false information. For example, Air Canada's chatbot provided misinformation to travelers, leading to confusion and complications. The airline was successfully sued as a result ([BBC](https://www.bbc.com/travel/article/20240222-air-canada-chatbot-misinformation-what-travellers-should-know)).
2. **Unsupported Claims:** The model generates baseless assertions, which can be especially harmful output from sensitive contexts such as healthcare or legal proceedings. For example, ChatGPT fabricated fake legal cases, leading to significant issues in court ([LegalDive](https://www.legaldive.com/news/chatgpt-fake-legal-cases-generative-ai-hallucinations/651557/)).
3. **Misrepresentation of Expertise:** The model gives the illusion of understanding complex topics, misleading users regarding its level of expertise. For example, chatbots have been found to misrepresent the complexity of health-related issues, suggesting uncertainty where there is none, which misled users into believing that unsupported treatments were still under debate ([KFF](https://www.kff.org/health-misinformation-monitor)).
4. **Unsafe Code Generation:** The model suggests insecure or non-existent code libraries, which can introduce vulnerabilities when integrated into software systems. For example, LLMs propose using insecure third-party libraries, which, if trusted without verification, led to security risks ([Lasso](https://www.lasso.security/blog/ai-package-hallucinations)).

### Prevention and Mitigation Strategies
1. **Retrieval-Augmented Generation (RAG):** Use Retrieval-Augmented Generation to enhance the reliability of model outputs by retrieving relevant and verified information from trusted external databases during response generation. This helps mitigate the risk of hallucinations and misinformation.
2. **Model Fine-Tuning:** Enhance the model with fine-tuning or embeddings to improve output quality. Techniques such as parameter-efficient tuning (PET) and chain-of-thought prompting can help reduce the incidence of misinformation.
3. **Cross-Verification and Human Oversight:** Encourage users to cross-check LLM outputs with trusted external sources to ensure the accuracy of the information. Implement human oversight and fact-checking processes, especially for critical or sensitive information. Ensure that human reviewers are properly trained to avoid overreliance on AI-generated content.
4. **Automatic Validation Mechanisms:** Implement tools and processes to automatically validate key outputs, especially output from high-stakes environments.
5. **Risk Communication:** First identify the risks and possible harms associated with LLM-generated content, then clearly communicate these risks and limitations to users, including the potential for misinformation.
6. **Secure Coding Practices:** Establish secure coding practices to prevent the integration of vulnerabilities due to incorrect code suggestions.
7. **User Interface Design:** Design APIs and user interfaces that encourage responsible use of LLMs, such as integrating content filters, clearly labeling AI-generated content and informing users on limitations of relibility and accuracy.  Be specific about intended field of use limitations.
8. **Training and Education:** Provide comprehensive training for users on the limitations of LLMs, the importance of independent verification of generated content, and the need for critical thinking. In specific contexts, offer domain-specific training to ensure users can effectively evaluate LLM outputs within their field of expertise.

### Example Attack Scenarios

**Scenario #1:** Attackers experiment with popular coding assistants for commonly hallucinated package names. Once they identify these frequently suggested but non-existent libraries, they publish malicious packages with those names to widely-used repositories. Developers, relying on the coding assistant's suggestions, unknowingly integrate these poised packages into their software. As a result, the attackers gain unauthorized access, inject malicious code, or establish backdoors, leading to significant security breaches and compromising user data.

**Scenario #2:** A company builds an LLM application to automatically summarize and publish news stories without sufficient human oversight. An attacker compromises the system by experimenting with malicious code, attempting to manipulate the news summaries to spread political, financial, or health-related misinformation. This misinformation is published as legitimate news articles, causing widespread confusion, influencing public opinion, and potentially leading to financial market disruptions or public health risks.

**Scenario #3:** A company puts out a chatbot for medical diagnosis without ensuring sufficient accuracy. The chatbot provides poor information, leading to harmful consequences for patients. As a result, the company is successfully sued for damages. In this case, the safety and security breakdown did not require a malicious attacker, but instead arose from the insufficient oversight and reliability of the LLM system.

### Reference Links
1. [AI Chatbots as Health Information Sources: Misrepresentation of Expertise](https://www.kff.org/health-misinformation-monitor/volume-05/): **KFF**
2. [Air Canada Chatbot Misinformation: What Travellers Should Know](https://www.bbc.com/travel/article/20240222-air-canada-chatbot-misinformation-what-travellers-should-know): **BBC**
3. [ChatGPT Fake Legal Cases: Generative AI Hallucinations](https://www.legaldive.com/news/chatgpt-fake-legal-cases-generative-ai-hallucinations/651557/): **LegalDive**
4. [Understanding LLM Hallucinations](https://towardsdatascience.com/llm-hallucinations-ec831dcd7786): **Towards Data Science**
5. [How Should Companies Communicate the Risks of Large Language Models to Users?](https://techpolicy.press/how-should-companies-communicate-the-risks-of-large-language-models-to-users/): **Techpolicy**
6. [A news site used AI to write articles. It was a journalistic disaster](https://www.washingtonpost.com/media/2023/01/17/cnet-ai-articles-journalism-corrections/): **Washington Post**
7. [Diving Deeper into AI Package Hallucinations](https://www.lasso.security/blog/ai-package-hallucinations): **Lasso Security**
8. [How Secure is Code Generated by ChatGPT?](https://arxiv.org/abs/2304.09655): **Arvix**
9. [How to Reduce the Hallucinations from Large Language Models](https://thenewstack.io/how-to-reduce-the-hallucinations-from-large-language-models/): **The New Stack**
10. [Practical Steps to Reduce Hallucination](https://newsletter.victordibia.com/p/practical-steps-to-reduce-hallucination): **Victor Debia**
11. [A Framework for Exploring the Consequences of AI-Mediated Enterprise Knowledge](https://www.microsoft.com/en-us/research/publication/a-framework-for-exploring-the-consequences-of-ai-mediated-enterprise-knowledge-access-and-identifying-risks-to-workers/): **Microsoft**