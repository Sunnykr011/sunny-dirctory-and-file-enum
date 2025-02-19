 sunny-dirctory-and-file-enum

Basic usage  
python3 web_enumerator.py -u https://example.com  

Custom wordlist  
python3 web_enumerator.py -u https://example.com -w /path/to/custom/wordlist.txt  

Specify output directory  
python3 web_enumerator.py -u https://example.com -o ./my_results

# How It Works:
The script initializes with the target URL, wordlist, and output directory.
It loads the wordlist and performs parallel enumeration using ThreadPoolExecutor.
It checks each path and logs valid URLs with their status codes and content types.
Results are saved in a JSON file in the specified output directory.
The script measures and displays the total time taken for the enumeration process.
This version is faster, more user-friendly, and ensures results are automatically saved for convenience. 


# Enhancements and Features:
Increased Thread Count: Increased the maximum number of threads to 50 for faster enumeration.
Error Handling: Added error handling for requests.RequestException to log errors when checking URLs.
Timing: Added timing to measure and display the total time taken for the enumeration process.
Verbose Output: Improved verbose output to include error messages and timing information.
Code Cleanup: Cleaned up the code for better readability and maintainability.
