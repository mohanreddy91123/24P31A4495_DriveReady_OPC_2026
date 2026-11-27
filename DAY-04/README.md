# Day 4 – Tools, Structured Output and Google Sheets

## Project: Sweet Crumbs Home Bakery

**Program:** One Person Company – Build Your Own AI Workforce  
**Day:** 04  
**Level:** Level 2 – Single Agent

---

## 1. Objective

The objective of Day 4 was to develop an AI agent that can use external tools, extract structured information from customer messages, validate orders and store order details in Google Sheets.

## 2. Technologies Used

- Python
- Google Colab
- LangChain
- LangGraph
- Groq LLM
- Pydantic
- Google Sheets
- gspread

## 3. Tools Implemented

The following tools were implemented:

| Tool | Purpose |
|---|---|
| `get_price` | Calculate the price of bakery products |
| `is_open` | Demonstrate opening-hours lookup |
| `get_menu` | Display available bakery products and prices |
| `log_order` | Save customer orders to Google Sheets |

## 4. Structured Output with Pydantic

Created an `Order` Pydantic model containing:

- Customer name
- Product name
- Quantity
- Pickup date
- Eggless requirement

Tested structured information extraction using five different customer messages.

## 5. Google Sheets Integration

Created a Google Spreadsheet named **Sweet Crumbs Orders**.

Implemented order storage using the `log_order` tool.

The spreadsheet contains:

- Order ID
- Customer name
- Product
- Quantity
- Unit price
- Total price
- Pickup date
- Eggless requirement
- Order status

Created a separate `Operations Demo` worksheet with eight sample orders.

### Google Sheets Link

[Open Sweet Crumbs Google Sheet](https://docs.google.com/spreadsheets/d/124_1Zj7bMk7Af0J64GSj8licWU722bKAxhsSbJUnxdk
)

## 6. Google Sheets Operations

Practised the following operations:

- Creating worksheets
- Inserting records
- Reading records
- Searching for customers
- Updating order information
- Formatting spreadsheet data

## 7. Agent Testing

Tested the agent with different customer requests, including:

- Valid product and quantity requests
- Unknown products
- Zero and negative quantities
- Missing order information
- Eggless requirements
- Multiple product requests
- Customer name changes
- Discount requests
- Delivery-related questions
- Prompt injection attempts

## 8. Pydantic Validation Testing

Tested six invalid order records.

Results:
- Invalid product rejected.
- Zero quantity rejected.
- Negative quantity rejected.
- Invalid quantity text rejected.
- Invalid eggless value rejected.
- Empty customer name was accepted, identifying an improvement required in validation.

## 9. Agent Trace Results

| Metric | Result |
|---|---:|
| Total tool calls | 2 |
| Total AI messages | 3 |

Used `pretty_print()` to inspect the agent execution trace.

## 10. Conclusion

Successfully implemented an AI agent with tool calling, structured output, Pydantic validation and Google Sheets integration.

The practical exercises demonstrated how an AI assistant can interact with external tools and manage structured customer order information.
