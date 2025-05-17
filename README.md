# FarmerWorld: Smart Plant Disease Detection and Crop Recommendation

FarmerWorld is a web application designed to assist farmers in identifying plant diseases early and making informed decisions about crop planting. By analyzing images of plant leaves, the application can detect diseases and suggest organic remedies. Additionally, it provides recommendations on which crops are best suited for planting in the current session based on various factors.

## Key Features

* **Plant Disease Detection:** Upload an image of a plant leaf, and the application will analyze it to identify potential diseases.
* **Organic Medicine Suggestions:** Based on the detected disease, the application provides recommendations for organic treatment methods.
* **Crop Recommendation:** Receive suggestions for suitable crops to plant in the current session, taking into account factors like season and potentially location (future enhancement).
* **User-Friendly Interface:** Simple and intuitive design for easy use by farmers.

## Technologies Used

* **Frontend:** HTML, CSS, JavaScript - For building the user interface.
* **Backend:** JavaScript (Node.js) - To handle server-side logic and API endpoints.
* **Image Processing & Disease Detection:** OpenCV (integrated with the backend), Convolutional Neural Network (CNN) algorithm.
* **Database:** MySQL - For storing plant disease information, organic remedies, and crop data.

## How it Works

1.  **Upload Image:** The farmer uploads a clear image of a plant leaf through the web interface.
2.  **Disease Analysis:** The backend receives the image and utilizes OpenCV for image processing. The processed image is then fed into a trained CNN algorithm to detect any signs of disease.
3.  **Disease Identification:** The application identifies the specific plant disease (if any) based on the CNN's analysis.
4.  **Organic Remedy Suggestion:** If a disease is detected, the application retrieves relevant organic treatment methods from the MySQL database and presents them to the user.
5.  **Crop Recommendation:** Separately, or potentially integrated, the application considers the current session (e.g., season) and suggests suitable crops for planting based on predefined data in the MySQL database.

## Getting Started (For Developers)

1.  **Prerequisites:**
    * Node.js and npm (Node Package Manager) installed.
    * MySQL database set up and running.
    * OpenCV library integrated with your Node.js environment.
    * Trained CNN model for plant disease detection (ensure the backend can access this model).

2.  **Clone the Repository:**
    ```bash
    git clone [YOUR_REPOSITORY_URL]
    cd farmerworld
    ```

3.  **Install Dependencies (Backend):**
    ```bash
    cd backend
    npm install
    ```

4.  **Database Configuration:**
    * Create a MySQL database for FarmerWorld.
    * Update the database connection details (host, user, password, database name) in your backend configuration files.
    * Run any necessary database migrations or seed scripts to set up the initial data.

5.  **Run the Backend:**
    ```bash
    cd backend
    npm start
    ```

6.  **Open the Frontend:** Navigate to the `frontend` directory and open the `index.html` file in your web browser. Ensure that the frontend JavaScript code is correctly configured to communicate with your running backend server (check API endpoints). You might need to run a local development server for the frontend depending on your setup.

## Potential Future Enhancements

* **Location-Based Crop Recommendations:** Integrate location data to provide more accurate crop suggestions.
* **Disease Severity Assessment:** Provide an estimate of the severity of the detected disease.
* **Integration with Weather Data:** Consider weather patterns for better crop recommendations.
* **User Accounts:** Allow farmers to save their plant history and preferences.
* **Image Database:** Build a larger database of plant leaf images for more accurate disease detection.
* **Mobile Application:** Develop a mobile app for easier image capture in the field.

## Contact

cs koushik koushikcs562@gmail.com
