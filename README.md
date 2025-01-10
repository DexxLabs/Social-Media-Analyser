# Social Media Performance Analysis - Socialens

## Objective

Build a user-friendly analytics module, **Socialens**, using Langflow and DataStax to analyze engagement data from mock social media accounts. This app provides insights into the performance of different post types, empowering users to optimize their content strategies.

---

## Tools Used

- **DataStax Astra DB**: For storing and managing engagement data efficiently.
- **Langflow**: For designing workflows and integrating GPT-based insights seamlessly.

---

## Dependencies

Make sure to install the following dependencies before running the project:

- **Streamlit**: For building the web interface.
- **LangChain Groq**: For GPT integration via Langflow.
- **Pandas**: For handling and processing datasets.
- **Plotly**: For creating interactive visualizations.
- **os**: For operating system interactions.
- **uuid**: For generating unique identifiers.
- **dotenv**: For managing environment variables.
- **Astrapy**: For interfacing with DataStax Astra DB.

Install these packages using pip:

```bash
pip install streamlit langchain-groq pandas plotly python-dotenv astrapy
```

---

## Features

### 1. Fetch Engagement Data

- Socialens uses a simulated dataset to mimic real-world social media engagement data. This includes metrics like:
  - Likes
  - Shares
  - Comments
  - Post types (e.g., carousel, reels, static images).
- The dataset is securely stored and queried using **DataStax Astra DB**.

### 2. Analyze Post Performance

Socialens processes and analyzes engagement data with the following capabilities:

- **Input Post Type**: Users can select a post type such as carousel, reels, or static images.
- **Performance Metrics**: Calculates average engagement metrics for the selected post type by querying the dataset in Astra DB.
- **Data Visualization**: Displays results in an easy-to-understand format using graphs and charts.

### 3. Provide Insights

With GPT integration in Langflow, Socialens generates actionable insights based on engagement data, such as:

- "Carousel posts have 20% higher engagement than static posts."
- "Reels drive 2x more comments compared to other formats."
- "Static images have consistent engagement but fewer shares compared to dynamic formats."

These insights help users make data-driven decisions to improve content strategy.

---

## How to Run Socialens

1. **Install Prerequisites**:
   - Ensure you have Python installed on your system.
   - Install Streamlit using:
     ```bash
     pip install streamlit
     ```

2. **Set Up the Project**:
   - Clone the repository or download the project files.
   - Navigate to the project directory using the terminal.

3. **Run the App**:
   - Start the application by running the following command:
     ```bash
     streamlit run app2.py
     ```
   - A local URL will be displayed in the terminal. Open this URL in your web browser to access Socialens.

4. **Configuration**:
   - Ensure your **DataStax Astra DB** credentials are correctly set up in the project configuration.
   - Verify that Langflow workflows are imported and functional as per the provided setup guide.

---

## Notes

- **Data Security**: Ensure Astra DB credentials are stored securely and not hard-coded in the app.
- **Customization**: Modify the dataset or workflows to tailor Socialens to specific use cases.

---

Socialens makes understanding social media engagement easy and actionable. Start optimizing your posts today!
