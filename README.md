- 👋 Hi, I’m **Abhishek Pal**
- 👨‍💼 I assume a position of a **Product Manager**
- 👀 I’m interested in **Flutter, Mobile App development, helping businesses grow in tech**
- 🌱 I’m currently learning **Fresh**, **GPT-4**
- 💞️ I’m looking to collaborate on **Any software/solutions in tech**


# Web Scraper

**Pre-requisite:**

*See Environment Variables section*


## **Installation Steps:**

**Step 1** : Install **python**, Recommended python version = 3.10, Install **pip**, recommended pip version : 23.0

Installation pertaining to the base OS.

**Step 2** :- Create a virtual environment

```
virtualenv venv
```

*OR*

Follow any of these docs, in case the given commands do not register for you

https://docs.python.org/3/library/venv.html

https://pypi.org/project/pipenv/

```
pip install pipenv
```

**Step 3:** Activate your current environment via pipenv:
```
pipenv shell
```

*OR*

Activate your environment via environment name:

```
source venv/bin/activate
```
* *here venv is your environment name*

**Step 4:** Install poetry via *pip*

```
pip install poetry
```

**Step 5:** Run poetry install to install depencies
```
poetry install
```

**Step 6:** Execute the scraper script
```
python app/main.py
```

**Step 7:** Set up a cron job to run this once a day at an approrpriate time. You would need to follow the base OS configuration pattern for that. 
## Environment Variables

To run this project

**Create a file named `aws-credentials.json`**

```
{
  "Access key ID" : "your_S3_access_key_here",
  "Secret access key": "your_S3_secret_key_here"
}
```
## Features

- Scrapes the below websites: <br />
    https://eprocure.gov.in/eprocure/app  <br />
    https://govtprocurement.delhi.gov.in/nicgep/app  <br />
    https://etender.up.nic.in/nicgep/app  <br />
    https://defproc.gov.in/nicgep/app   <br />
    https://etenders.gov.in/eprocure/app   <br />

- Scheduler for getting the data fetched to the db 2 hours after the scraping completes.
- CLI updates for the current job.
- Uploads the files to the S3 bucket with the folder structure in *website/yy/mm/dd/tenderID/file.ext* format


## Authors

- [@abhishek pal](https://github.com/abhishekpal-nexg)


Powered by 

<img align="left" width="80" src="https://nexgeniots.com/wp-content/uploads/2021/11/NexGen-Logo_512x380.svg">
<!---
abhishekpal-nexg/abhishekpal-nexg is a ✨ special ✨  epository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
