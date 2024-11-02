# Word Counter Program

def count_words(text):
    """
    Function to count the number of words in a given text.
    :param text: str - The input text provided by the user.
    :return: int - The word count.
    """
    # Splitting the text by spaces to count words and filtering out any empty strings
    words = text.split()
    return len(words)

def main():
    """
    Main function to handle user input and display word count.
    """
    print("Welcome to the Word Counter Program!")
    
    # Taking input from the user
    user_input = input("Please enter a sentence or paragraph: ").strip()
    
    # Checking if the input is empty
    if not user_input:
        print("Error: You entered an empty input. Please provide some text.")
    else:
        # Calling the count_words function to get the word count
        word_count = count_words(user_input)
        
        # Displaying the word count to the user
        print(f"The number of words in the given text is: {word_count}")
        #Run the program
main()
