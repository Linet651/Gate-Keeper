import time


# This function simulates opening the electric gate
def open_gate():
    print("opening gate...")
    time.sleep(2)
    print("gate is now open!")


def check_code(user_code, valid_code):
    if user_code == valid_code:
        return True
    return False


def main():
    valid_code = "1234"
    print("welcome to the parking lot Gate System!")

    user_code = input("Please enter the access code to open the gate: ")
    if check_code(user_code, valid_code):
        print("code accepted!")
        open_gate()
    else:
        print("Invalid code! Access denied.")


if __name__ == "__main__":
    main()
