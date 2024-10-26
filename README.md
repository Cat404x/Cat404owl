# Cat404owl
## Social Media Scraper Setup

To run the script, ensure you have all the necessary components set up and configured correctly. Here's a step-by-step guide to help you execute it successfully:

### Prerequisites

1. **Install Python**: Ensure Python is installed on your system. You can download it from [python.org](https://www.python.org/).

2. **Install Required Packages**: Use pip to install the necessary Python packages. Open a terminal or command prompt and run:
   ```bash
   pip install selenium requests beautifulsoup4 pandas
   ```

3. **ChromeDriver Setup**: 
   - Download the ChromeDriver that matches your installed version of Google Chrome from the [ChromeDriver site](https://sites.google.com/corp/chromium.org/driver/).
   - Ensure that `chromedriver` is in your system's PATH or specify its path directly in your script initialization if needed.
   
4. **Tor Network (Optional)**:
   - Install Tor on your machine and ensure it's running. On most systems, this can be done using:
     ```bash
     tor
     ```
   - You can check if Tor is working by setting the `use_tor` parameter to `True` in the script if you desire to route traffic through the Tor network.

### Script Execution

1. **Save the Script**: Save your Python script to a file, e.g., `data_extractor.py`.

2. **Run the Script**: In your terminal or command prompt, navigate to the directory where your script is saved and execute:
   ```bash
   python data_extractor.py
   ```

3. **Observing Output**:
   - The script will open a browser window and perform the tasks specified: scraping a website, performing a search, and extracting product info.
   - Results will be saved to CSV files named `paragraphs.csv`, `search_results.csv`, and `product_info.csv`.

### Troubleshooting

- **WebDriver Issues**: Ensure that the ChromeDriver version matches the Google Chrome version. If necessary, specify the path to the `chromedriver` executable explicitly in the initialization:
  ```python
  self.driver = webdriver.Chrome(executable_path='/path/to/chromedriver', options=chrome_options)
  ```

- **Tor Connectivity**: If opting to use Tor, make sure it's actively running and listening on the correct port. You might need to check the Tor network logs for any connectivity issues.

- **SSL Errors**: If you encounter SSL certificate errors, consider skipping SSL verification in your requests by modifying:
  ```python
  requests.get(url, verify=False)
  ```
  However, do this with caution as it might expose you to security risks.

Following these steps should help you run your script efficiently and handle basic web scraping and search tasks while allowing you the flexibility to integrate Tor for private browsing when required.


This message has been generated by Nova - download it for free:
https://novaappai.page.link/zFQ7yozWcneFZNLb8
