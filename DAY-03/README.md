# Day 3 – Your First AI Agent with LangChain

## Project
**Sweet Crumbs Home Bakery – AI Customer Assistant**

## Objective
Build an AI-powered bakery customer assistant using LangChain. The assistant answers customer questions about products, prices, eggless options and ordering requirements.

## Topics Covered
1. Chatbot vs AI Agent
2. Four Parts of an Agent
3. Agent Loop – Think, Act, Observe, Repeat
4. Three Levels of AI
5. Agent or Not?
6. Introduction to LangChain
7. LangChain Models, Templates and Chains
8. Testing an AI Assistant

## Practical Implementation

- Created a bakery customer assistant using LangChain.
- Implemented conversation history using memory.
- Created a custom system prompt for Sweet Crumbs Home Bakery.
- Tested customer questions about prices, eggless cakes and ordering requirements.
- Created Python functions for price calculation and order notice validation.
- Explored LangChain's `create_agent` interface.
- Created a customer test dataset containing 10 questions.

## Business Rules

- Plum cake – ₹500
- Chocolate cake – ₹650
- Cupcake – ₹80
- Orders require 24 hours' notice.
- All cakes have eggless versions.
- Never promise a delivery time.
- For unknown information, say: "I'll check with the owner."

## Testing Results

| Temperature | Test Run | Result |
|---|---|---|
| 0.3 | Initial test | 20/20 (100%) |
| 1.0 | Run 1 | 15/20 (75%) |
| 1.0 | Run 2 | 15/20 (75%) |
| 0.3 | Improved prompt | Result pending recording |

## Python Functions

**1. `get_price()`**
- Calculates the total price of a menu item.
- Validates the product and quantity.

**2. `check_order_notice()`**
- Checks whether an order meets the 24-hour notice requirement.

## Agent or Not?

| Business Task | Approach |
|---|---|
| Calculate the total price for 5 chocolate cakes | Plain Python |
| Create a Christmas cake promotional post | One LLM Call |
| Handle a customer order using tools and collect missing details | AI Agent |

## Files

- `Sweet_Crumbs_Day3.ipynb` – Practical implementation and experiments.
- `tests.csv` – Dataset containing 10 customer test questions and expected keywords.

## Conclusion

Day 3 introduced AI agents and LangChain. I developed a bakery customer assistant, tested its responses, compared temperature settings, created Python functions and explored how agents can use tools to complete customer tasks.

## Status
Completed – Day 3 practical work and documentation.
