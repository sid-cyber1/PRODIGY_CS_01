def caesar_cipher(text, shift):
    result = ""
    for char in text:
        if char.isalpha():
            shift_amount = 65 if char.isupper() else 97
            result += chr((ord(char) - shift_amount + shift) % 26 + shift_amount)
        else:
            result += char
    return result

message = input("Enter the message to encrypt/decrypt: ")
shift_value = int(input("Enter the shift value: "))

encrypted_message = caesar_cipher(message, shift_value)
print("Encrypted message:", encrypted_message)

decrypted_message = caesar_cipher(encrypted_message, -shift_value)
print("Decrypted message:", decrypted_message)
