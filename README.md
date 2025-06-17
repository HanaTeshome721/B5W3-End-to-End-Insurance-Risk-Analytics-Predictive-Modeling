 Task 2: Data Version Control (DVC)
📌 Task Objective
Establish a reproducible and auditable data pipeline using DVC (Data Version Control) to ensure that all datasets used in the project are version-controlled, traceable, and reproducible—meeting compliance standards required in regulated industries like finance and insurance.

✅ Steps Completed
1. 📦 DVC Installation
bash
Copy
Edit
pip install dvc
DVC was successfully installed in the project environment.

2. 🏁 DVC Initialization
bash
Copy
Edit
dvc init
git commit -m "Initialize DVC for project tracking"
This created the .dvc/ directory and updated .gitignore to prevent large files from being pushed to Git.

3. 🗃️ Local Remote Storage Setup
bash
Copy
Edit
mkdir ../dvc-storage
dvc remote add -d localstorage ../dvc-storage
A local DVC remote was created and configured for offline reproducibility.

4. 📂 Data Tracking with DVC
bash
Copy
Edit
dvc add data/MachineLearningRating_v3.parquet
The main dataset was added to DVC, generating a .dvc file to track its metadata.

5. ✅ Committing DVC Files to Git
bash
Copy
Edit
git add data/MachineLearningRating_v3.parquet.dvc .gitignore .dvc/config
git commit -m "Track dataset using DVC and configure local remote"
DVC metadata and tracking files were committed to the Git repository.

6. 🚀 Data Push to Remote
bash
Copy
Edit
dvc push
Dataset successfully pushed to the configured local remote storage.

7. ♻️ Reproducibility Test (Optional)
To reproduce the data from a fresh clone:

bash
Copy
Edit
git clone <repo-url>
cd <repo>
dvc pull
This command restores the exact dataset version from the remote, ensuring reproducibility.

📂 DVC Tracked Files
data/MachineLearningRating_v3.parquet.dvc — Metadata for the dataset.

.dvc/config — Remote storage configuration.

.gitignore — Prevents raw data from being pushed to Git.

🧪 Notes & Compliance
✅ No raw data is pushed to GitHub.

✅ Data versioning is fully functional.

✅ dvc pull restores datasets consistently.

