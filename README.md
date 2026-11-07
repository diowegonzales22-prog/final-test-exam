while True:

    print("=" * 40)
    print("  FUNDAMENTALS OF PROGRAMMING LESSONS")
    print("=" * 40)

    print("")
    print("Hello sir! welcome to python tutorial system.")
    print("How can I help you today?")

    print("")
    print("What chapter do you want to study?")
    print("[1] Chapter 1 - Introduction to programming")
    print("[2] Chapter 2 - Python basic syntax")
    print("[3] Chapter 3 - Arithmetic operators and expressions")
    print("[4] exit:")
    print("")

    chapter = input("Enter chapter number: ")
    print("")

    if chapter == "1":

        print("Chapter 1: Introduction to programming")
        print("[1] What is a programming language?")
        print("[2] Why learn Python?")
        print("[3] What do you need to start Python?")
        print("[4] exit:")
        print("")

        lesson = input("Enter lesson number: ")

        if lesson == "1":
            print("Lesson: What is a programming languange?")
            print("A programming language is a formal vocabulary and set of grammatical rules (syntax) used to write computer programs that humans can read and machines can execute.")
            print("")
            print("Example code:")
            print('print("Hello, world")')
            print("")
            print("Output:")
            print("Hello, world!")

        elif lesson == "2":
            print("Lesson: Why learn Python?")
            print("Python is simple and easy to learn. It has readable syntax and is versatile. It also has a huge community.")
            print("")
            print("Example code:")
            print('print("Python is easy to learn!")')
            print("")
            print("Output:")
            print("Python is easy to learn!")

        elif lesson == "3":
            print("Lesson: What do you need to start Python?")
            print("You need Python and a code editor or IDE. Examples are PyCharm, VS Code, and Jupyter Notebook.")
            print("")
            print("Example code:")
            print('print("I am ready to learn Python!")')
            print("")
            print("Output:")
            print("I am ready to learn Python!")

        else:
            print("Invalid lesson number!")

    elif chapter == "2":

        print("Chapter 2: Python basic syntax")
        print("What lesson do you want to learn?")
        print("[1] What is Python syntax?")
        print("[2] Python is case-sensitive")
        print("[3] Indentation")
        print("")

        lesson = input("Enter lesson number: ")

        if lesson == "1":
            print("Lesson: What is Python syntax?")
            print("Syntax refers to the set of rules that defines how a Python program is written and structured.")
            print("")
            print("Example code:")
            print('name = "diowe"')
            print("print(name)")
            print("")
            print("Output:")
            print("diowe")

        elif lesson == "2":
            print("Lesson: Python is case-sensitive")
            print("Python treats uppercase and lowercase letters differently. Name and name are not the same.")
            print("")
            print("Example code:")
            print('name = "diowe"')
            print("print(name)")
            print("")
            print("Output:")
            print("diowe")

        elif lesson == "3":
            print("Lesson: Indentation")
            print("Indentation refers to the spaces at the beginning of a line of code. It defines blocks of code in Python.")
            print("")
            print("Example code:")
            print("age = 18")
            print("if age >= 18:")
            print('    print("Adult")')
            print("")
            print("Output:")
            print("Adult")

        else:
            print("Invalid lesson number!")


    elif chapter == "3":

        print("Chapter 3: Arithmetic operators")
        print("What lesson do you want to learn?")
        print("[1] What are arithmetic operators?")
        print("[2] Arithmetic operators in Python")
        print("[3] Expression in Python")
        print("[4] PEMDAS")
        print("")

        lesson = input("Enter lesson number: ")

        if lesson == "1":
            print("Lesson: What are arithmetic operators?")
            print("Special symbols used to perform mathematical calculations on numbers (operands).")
            print("")
            print("Example code:")
            print("print(12 + 12)")
            print("")
            print("Output:")
            print("24")

        elif lesson == "2":
            print("Lesson: Arithmetic operators")
            print("+ Addition")
            print("- Subtraction")
            print("* Multiplication")
            print("/ Division")
            print("// Floor Division")
            print("% Modulus")
            print("** Exponentiation")
            print("")
            print("Example code:")
            print("a = 10")
            print("b = 5")
            print("print(a + b)")
            print("")
            print("Output:")
            print("15")

        elif lesson == "3":
            print("Lesson: Expression in Python")
            print("An expression is a combination of values, variables, and operators that the interpreter evaluates down to a single value.")
            print("")
            print("Example code:")
            print("a = 12")
            print("b = 12")
            print("result = a + b")
            print("print(result)")
            print("")
            print("Output:")
            print("24")

        elif lesson == "4":
            print("Lesson: PEMDAS")
            print("Python follows the order of operations:")
            print("P - Parentheses")
            print("E - Exponents")
            print("M - Multiplication")
            print("D - Division")
            print("A - Addition")
            print("S - Subtraction")
            print("")
            print("Example code:")
            print("result = 1 + 3 * 4")
            print("print(result)")
            print("")
            print("Output:")
            print("13")

        else:
            print("Invalid lesson number!")

    else:
        print("Invalid chapter number!")

    print("")
    repeat = input("Do you want to study another lesson? (yes/no): ")

    if repeat.lower() == "yes":
        print("")
        continue
    else:
        print("")
        print("Thank you for using Python Tutorial System!")
        break
