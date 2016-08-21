# pin_checker

a = []


def enter_pin():
    pin_input = input("Enter Pin: ")
    check_pin(pin_input)

def enter_puk():
    puk_input = input("Enter PUK")
    check_puk(puk_input)

def check_puk(puk):
    if puk == "2345":
        print("Sim unlocked")

    else:
        print(a)
        if len(a) < 2:
            a.append(1)
            enter_puk()
        elif enter_puk:
            print("Number of puk exceeded")
            print("Call 911 for more info")


def check_pin(pin):
    if pin == "1234":
        print("correct pin")

    else:
        print(a)
        if len(a) < 2:
            a.append(1)
            enter_pin()
        else:
            print("Sorry number of pin retries exceeded")
            enter_puk()

enter_pin()



