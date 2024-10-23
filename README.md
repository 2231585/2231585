import webbrowser

def open_link():
    # Prompt the user to enter a URL
    url = input("Enter the URL you want to open: ")
    
    # Validate if the input is not empty
    if url:
        try:
            # Open the link in the default browser
            webbrowser.open(url)
            print(f"Opening {url} in your default web browser...")
        except Exception as e:
            print(f"An error occurred: {e}")
    else:
        print("No URL provided. Please enter a valid URL.")

# Run the function
if __name__ == "__main__":
    open_link()
