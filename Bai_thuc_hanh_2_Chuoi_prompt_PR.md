#  PROMPT VIẾT BÀI PR CÔNG NGHỆ

**Product:** Enterprise AI Chatbot Solution
**Goal:** Produce a high-quality, in-depth 1000-1500 word PR article using a 3-step Prompt Chain.

---

### PROMPT 1 - Nghiên cứu khách hàng và phân tích pain points
*Câu lệnh để tạo dữ liệu đầu vào.*

**[C] Context:** 
Act as a Senior B2B Tech Product Marketer and Market Researcher. You have deep expertise in enterprise software solutions and customer behavior analysis.

**[R] Request:** 
Analyze the target audience for a newly launched "Enterprise AI Chatbot Solution" and generate a comprehensive list of their core pain points.

**[E] Explanation:** 
- Identify the key decision-makers (e.g., Customer Service Directors, CTOs, COOs).
- Discover at least 5 distinct pain points they are currently facing with traditional customer service methods (e.g., high operational costs, slow response times, 24/7 unavailability, inconsistent answers).
- Explain briefly how an AI Chatbot can resolve each pain point.
- **Data Transfer Rule:** At the end of your response, summarize these pain points into a structured list labeled `[PAIN_POINTS_DATA]` so I can use it for the next step.

**[A] Action / Arguments:** 
- Product: Enterprise-grade AI Chatbot capable of natural language processing, CRM integration, and multi-language support.
- Industry: B2B, E-commerce, Finance, or SaaS.

**[T] Tone / Type:** 
Professional, analytical, and data-driven. Output format must be a clear Markdown table and bulleted lists.

---

### PROMPT 2 - SEO Gợi ý dàn ý bài PR
*Sử dụng dàn ý từ prompt 1 .*

**[C] Context:** 
Act as a Lead Content Strategist and SEO Expert. You excel at structuring long-form B2B PR articles that capture attention and rank well on search engines.

**[R] Request:** 
Based on the `[PAIN_POINTS_DATA]` generated in the previous step, create a highly detailed, SEO-optimized outline for a PR article (target length: 1000 - 1500 words).

**[E] Explanation:** 
The outline must strictly follow standard PR and SEO structures:
1. **Headline:** Propose 3 catchy, click-worthy title options.
2. **Lead (Introduction):** Hook the reader by directly addressing the top pain points.
3. **Body Paragraphs (H2, H3):** 
   - Map each section to a specific pain point and the AI Chatbot's corresponding solution.
   - Include a section for "Key Features" and "Expected ROI/Benefits".
4. **Conclusion & CTA:** A strong Call-To-Action urging businesses to book a demo.
- **Data Transfer Rule:** Output the final approved structure under the tag `[ARTICLE_OUTLINE]` to feed into the final writing phase.

**[A] Action / Arguments:** 
- Input Data: `[Paste the PAIN_POINTS_DATA from Step 1 here]`
- Target Keywords: AI Chatbot for Enterprise, automate customer service, AI customer support, reduce operational costs.

**[T] Tone / Type:** 
Structured, hierarchical, and strategic. Format as a Markdown outline using bullet points and heading tags (H1, H2, H3).

---

### PROMPT 3 - Viết bài PR dài 1000 - 1500 từ
*Sử dụng dàn ý từ Prompt 2 để tạo nội dung dài.*

**[C] Context:** 
Act as an Expert B2B Tech Copywriter and PR Specialist. You write compelling, trustworthy, and authoritative content that converts readers into leads.

**[R] Request:** 
Write the complete PR article (1000 - 1500 words) based exactly on the `[ARTICLE_OUTLINE]` provided. 

**[E] Explanation:** 
- Expand on each H2 and H3 thoroughly to ensure the article reaches the target word count without fluff.
- Naturally weave in the target SEO keywords.
- Address the pain points with empathy before presenting the AI Chatbot as the ultimate solution.
- **Continuity & Token Limit Rule:** Because this is a long article, if you hit your maximum token limit and stop generating mid-sentence, I will type the exact command: **`CONTINUE_WRITING`**. When you see this command, you must seamlessly resume writing from the exact word where you left off, maintaining the exact same tone and formatting without writing any introductory or repeating sentences.

**[A] Action / Arguments:** 
- Input Data: `[Paste the ARTICLE_OUTLINE from Step 2 here]`
- Tone Constraint: Do not change the tone across different sections. Keep it consistently professional, authoritative, yet engaging.

**[T] Tone / Type:** 
Persuasive, authoritative B2B PR tone. Format using clean Markdown with bolded key phrases, H2/H3 tags, and short, readable paragraphs.
