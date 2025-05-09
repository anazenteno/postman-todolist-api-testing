# ✅ TODOIST  
Instructions to Set Up and Run Automated API Tests Using Postman

## 🔧 Prerequisites

1. **Postman Installation**  
   Make sure you have the latest version of Postman installed.  
   Download it from: [https://www.postman.com/](https://www.postman.com/)

2. **Node.js v16+ and Newman**  
   Install Node.js from: [https://nodejs.org/en](https://nodejs.org/en)  
   Newman is Postman's CLI tool and can be installed using npm:

   ```bash
   npm install -g newman
   ```

   To generate HTML reports, install the Newman HTML Extra reporter:

   ```bash
   npm install -g newman-reporter-htmlextra
   ```

## 📁 Project Repository

1. Clone this repository:

   ```bash
   git clone https://github.com/anazenteno/repository-postman.git
   cd repository-postman
   ```

## 🚀 Setting Up in Postman

1. **Import the Collection and Environment:**
   - Open Postman.
   - Click **Import** (top left).
   - Select the two `.json` files (collection and environment).
   - Click **Import**.

## 🧪 Running Tests in Postman

1. **Manual Execution:**
   - Select the imported collection.
   - Click the **3 dots** next to the collection name → **Edit**.
   - Go to the **Authorization** tab.
   - Set the type to **Bearer Token**.
   - Enter your Todoist API token (found in your Todoist account):
     - `Account > Settings > Integrations > Developer`
   - Click **Save**.
   - Click **Run** to open the **Collection Runner**.
   - Select the `Todoist-Tasks` environment.
   - Click **Start Run** to execute the tests.

## 📊 Generating HTML Reports with Newman

1. **Edit the batch script `collection-todoist.bat` using any text editor:**

   ```bash
   set POSTMAN_API_KEY=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  # Your Postman API Key  
   set COLLECTION_UID=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX   # Collection UID  
   set ENVIRONMENT_UID=XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX  # Environment UID
   ```

2. **Notes:**
   - Generate your API Key from your Postman account.
   - To get your **Collection UID**, send a request to:  
     `https://api.getpostman.com/collections`  
   - To get your **Environment UID**, send a request to:  
     `https://api.getpostman.com/environments`  
   - Use your Postman API Key for authentication in both cases.

3. **Run the report:**
   - Double-click the `collection-todoist.bat` script.
   - The script will automatically fetch the latest version of the collection and environment from Postman.
   - It will run the tests and generate an HTML report in the same folder.
   - Look for the browser icon file (HTML) and open it to view the report.

## 📝 Additional Notes

- **Documentation**: For advanced usage, check the official docs:  
  - [Postman Documentation](https://learning.postman.com/docs/)  
  - [Newman Documentation](https://www.npmjs.com/package/newman)

- **Support**:  
  If you run into issues or have questions, feel free to contact me.
