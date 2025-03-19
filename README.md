# python-assignmrnt
week 1 python assignment



def simple_calculator():
    try:
        num1 = float(input('Enter the first number: '))
        num2 = float(input('Enter the second number: '))
        operation = input('Enter an operation (+, -, *, /): ')

        if operation == '+':
            result = num1 + num2
        elif operation == '-':
            result = num1 - num2
        elif operation == '*':
            result = num1 * num2
        elif operation == '/':
            if num2 != 0:
                result = num1 / num2
            else:
                return 'Error: Division by zero is not allowed.'
        else:
            return 'Invalid operation. Please enter one of +, -, *, /.'

        return f'{num1} {operation} {num2} = {result}'

    except ValueError:
        return 'Invalid input. Please enter valid numbers.'


# Run the calculator
print(simple_calculator())
