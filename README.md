# Equipment Rental Email Processing System

This project is an automated system for processing customer emails related to equipment rental inquiries, reviews, and assistance requests.

## Features

- Email classification (inquiry, review, assistance, or other)
- Automated handling of equipment rental inquiries
- Review sentiment analysis and response generation
- Assistance request handling with FAQ search
- Automated forwarding to customer service for unclassified emails

## Prerequisites

- Python 3.7+
- Groq API key
- SMTP-enabled email account for forwarding emails

## Installation

1. Clone this repository:
```git clone
https://github.com/yourusername/equipment-rental-email-system.git
```
```
cd equipment-rental-email-system
```

2. Install required packages

3. Set up environment variables

## Usage

1. Ensure you have a SQLite database named `equipment_rental.db` with the necessary tables.

2. Prepare a `faq.txt` file with frequently asked questions and answers.

3. Run the main script:
```
python main.py
```
4. The system will process incoming emails, classify them, and respond accordingly.

## Functions

- `classify_email(email_content)`: Classifies the email into categories.
- `handle_inquiry(email_content)`: Processes equipment rental inquiries.
- `handle_review(email_content)`: Analyzes and responds to customer reviews.
- `handle_assistance(email_content)`: Provides assistance based on FAQ or escalates to customer service.
- `process_email(email_content)`: Main function to process incoming emails.
- `forward_to_customer_service(email_content)`: Forwards emails to customer service.

## Configuration

- Adjust the SMTP server settings in `forward_to_customer_service()` function if not using Gmail.
- Modify the customer service email address in the same function.

## Security Notes

- Ensure that sensitive information (API keys, email credentials) is stored securely and not exposed in the code.
- Consider using a dedicated email sending service for production environments.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
