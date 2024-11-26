# Instructions

# Instructions

---

## Step 3: Clone the ICOAR Repository

1. Download the project files by cloning the GitHub repository:
   - `git clone https://github.com/CUSecLab/ICOAR.git`
2. Navigate to the project directory:
   - `cd ICOAR`

---

## Step 4: Install System Dependencies

1. Update your system’s package list and install necessary tools:
   - ```bash
     apt-get update && apt-get install -y \
         build-essential \
         curl \
         software-properties-common \
         wget \
         git \
         && rm -rf /var/lib/apt/lists/*
     ```

---


## Step 5: Build Frontend Components

### Part 1: Build the citations Component
1. Navigate to the citations directory:
   - `cd ./citations`
2. Install dependencies and build the module:
   - `npm install --legacy-peer-deps`
   - `npm run build`

### Part 2: Build the corousel Component
1. Navigate to the corousel directory:
   - `cd ../corousel`
2. Install dependencies and build the module:
   - `npm install --legacy-peer-deps`
   - `npm run build`

### Part 3: Build the header_tab Component
1. Navigate to the header_tab directory:
   - `cd ../header_tab`
2. Install dependencies and build the module:
   - `npm install --legacy-peer-deps`
   - `npm run build`

### Part 4: Build the header_tab2 Component
1. Navigate to the header_tab2 directory:
   - `cd ../header_tab2`
2. Install dependencies and build the module:
   - `npm install --legacy-peer-deps`
   - `npm run build`

### Part 5: Build the header_tab3 Component
1. Navigate to the header_tab3 directory:
   - `cd ../header_tab3`
2. Install dependencies and build the module:
   - `npm install --legacy-peer-deps`
   - `npm run build`

### Final Step: Return to the Main Project Directory
1. Navigate back to the main directory:
   - `cd ..`

---

## Step 6: Install Backend Dependencies with Poetry

1. Return to the main project directory:
   - `cd ..`
2. Configure Poetry to install dependencies without creating a virtual environment:
   - `poetry config virtualenvs.create false`
3. Install required backend dependencies:
   - `poetry install --only main --no-interaction --no-ansi`

---

## Step 7: Create Necessary Directories

1. Create a directory named `model`:
   - `mkdir -p /model`
2. Create another directory named `models`:
   - `mkdir -p /models`

---

## Step 8: Install Additional Python Packages

1. Install **gdown** to download files from Google Drive:
   - `pip install gdown`
2. Install `replicate`, used for replication tasks:
   - `pip install replicate`
3. Install `pyLDAvis`, used for data visualization:
   - `pip install pyLDAvis`

---

## Step 9: Download Pre-trained Model Files

1. Use **gdown** to download the necessary model files:
   - `gdown 1D-DK__8fRpIwt1Xqe5xRg2brNrjVIqYx`

---

## Step 10: Set Up Application Data

1. Create a directory for storing images within the app’s data folder:
   - `mkdir -p /data/images/image`

---

## Step 11: Run the Application

1. Launch the application using Streamlit:
   - `streamlit run Home.py`
2. Open the provided link in your web browser to access the app.

---

## Troubleshooting

- **Dependency Errors**: Ensure all required tools and libraries are installed.
- **Command Not Found**: Verify your system PATH includes Python, Node.js, and other tools.
- **Windows Users**: Use WSL (Windows Subsystem for Linux) if commands like `apt-get` are unavailable.

---

