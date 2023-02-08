# payment-gateway-code-
payment gateway code that can accept payments in multiple currencies using Python:

class PaymentGateway:
    def __init__(self):
        self.supported_currencies = ['USD', 'EUR', 'GBP', 'INR']

    def accept_payment(self, amount, currency):
        if currency not in self.supported_currencies:
            return "Error: Unsupported currency"
        else:
            # process the payment in the specified currency
            # ...
            return "Payment of {} {} accepted".format(amount, currency)

payment_gateway = PaymentGateway()
print(payment_gateway.accept_payment(100, 'USD'))
print(payment_gateway.accept_payment(100, 'JPY'))
