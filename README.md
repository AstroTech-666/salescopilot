<p align="center">
  <video width="70%" controls>
    <source src="healthcare.mp4" type="video/mp4">
    100X Your Healthcare Admin with Virtual Workforce Demo
  </video>
</p>

# 🚀 SalesCopilotPro - Your Open-Source AI Sales Agent
---

**SalesCopilotPro** is revolutionizing the way businesses sell with an AI-powered sales agent that can handle voice, email, and text communications! Whether you're chatting on SMS, WhatsApp, WeChat, or even voice calls, SalesCopilotPro is here to boost your sales game. And the best part? It's *context-aware*, meaning it understands exactly where you are in the conversation and tailors its responses accordingly.

### What’s New:
🔥 **AI Sales Agents now ACTUALLY sell!**  
🚀 **Stripe payment links** now generated automatically for seamless transactions.  
🛠️ Your AI Sales Agent can now *lookup products* from a product catalog!

---

### 🌟 **Features**:  
**1. Contextual Understanding** – SalesCopilotPro adapts to your sales process:
- **Introduction**: Make a great first impression!
- **Qualification**: Find the right prospects.
- **Value Proposition**: Show them why you rock.
- **Needs Analysis**: Discover their pain points.
- **Solution Presentation**: Pitch your product as the solution.
- **Objection Handling**: Address concerns like a pro.
- **Close**: Seal the deal!

**2. Business & Product Knowledge** – Access your business info to minimize errors and confusion!

**3. Close Sales** – SalesCopilotPro now *generates Stripe payment links* to complete transactions! 💳

**4. Multi-Channel Support** – Voice, text, email, you name it. SalesGPT's got it covered.

**5. Connect to Any Data System** – Integrate with your current tools via **Mindware**.

**6. Automated Email Communication** – Personalized emails & follow-ups to keep prospects engaged.

**7. Calendly Scheduling** – Set up meetings with ease.

**8. Flexibility** – Use *ANY* LLM with LiteLLM to power your AI Sales Agent! 😎

---

### 🛠️ **Quick Start**:
Getting started is super easy:
1. **Install Dependencies**:
    ```bash
    pip install salesgpt
    ```

2. **Setup AI Sales Agent**:
    ```python
    from salesgpt.agents import SalesGPT
    from langchain_community.chat_models import ChatLiteLLM

    llm = ChatLiteLLM(model_name="gpt-4")

    sales_agent = SalesGPT.from_llm(
        llm, 
        product_catalog="examples/sample_product_catalog.txt", 
        salesperson_name="Ted Lasso", 
        company_name="Sleep Haven", 
        company_business="Sleep Haven is a premium mattress company."
    )
    sales_agent.seed_agent()
    sales_agent.step()  # Start the conversation!
    ```

---

### 🚀 **Advanced Setup**:
For those who like to customize:
- **Using Docker**: Start SalesCopilotPro in a secure, isolated environment.
    ```bash
    docker-compose up -d
    ```
- **Direct UI Launch**: Run it locally for a seamless experience.
- **Terminal**: Run SalesCopilotPro right from your terminal.
    ```bash
    python run.py --verbose True --config examples/example_agent_setup.json
    ```

---
