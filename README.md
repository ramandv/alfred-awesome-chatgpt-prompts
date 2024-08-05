##Alfred Workflow: CSV to JSON Script Filter

This Alfred workflow uses a Python script to fetch and process CSV data from a specified URL, configured via an environment variable. The script converts the CSV data into JSON format suitable for Alfred's script filter and includes a caching mechanism for optimal performance.

### Features

- **Dynamic URL Configuration:** The URL for fetching CSV data is specified through the `PROMPTS_URL` environment variable, allowing easy updates without modifying the script.
- **Data Processing:** Transforms CSV data into JSON format with fields compatible with Alfred's script filter.
- **Caching:** Caches results for 24 hours to reduce redundant data fetching and improve efficiency.

### Setup

1. **Configure Environment Variable:**
    
    - Set the environment variable `PROMPTS_URL` in your Alfred workflow configuration to the URL of the CSV file.
2. **Script Execution:**
    
    - The script retrieves the CSV data from the `PROMPTS_URL`, processes it, and generates the required JSON format for Alfred's script filter.
3. **Cache Duration:**
    
    - Results are cached for 24 hours to prevent frequent data retrieval and enhance performance.

### Usage

- Integrate this script into an Alfred workflow to utilize the processed CSV data within Alfred’s interface.
- The script is designed for simplicity and flexibility, making it adaptable to various CSV data sources and use cases.

### Requirements

- Python 3.x
- Python’s built-in libraries (`csv`, `json`, `urllib`, and `os`)
