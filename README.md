# Website Deployment Process

A general website deployment checklist. This check list should cover the deployment of most website classes.

## Contents

1. Introduction
2. Assumptions
3. Preflight Checks
4. Deployment
    * Method 1. Git Deployment
    * Method 2. FTP Deployment
5. Post Deployment
6. End.

## 1. Introduction

## 2. Assumptions

## 3. Preflight Checks

This section walks through the steps we take **before** deploying any website.

1. [  ] Get client hosting information 
2. [  ] Go through **QA Checklist**
  1. [  ] `Git Merge` to Staging
  2. [  ] Note all URLS/paths that will need changing when live ( *the odd static url* )
3. [  ] Backup **everything**
  1. [  ] Backup **local/dev DB** 
  2. [  ] Backup **local/dev site** 
  3. [  ] Backup **Remote/existing DB** 
  4. [  ] Backup **Remote/existing site** 
4. [  ] Develop **Deployment Plan**.
5. [  ] Develop **Production QA Plan**.
6. [  ] Discuss **Deployment Plan** with key stakeholders.
7. [  ] If possible, set live site to maintenance mode.
8. [  ] Notify key stakeholders that deployment is in process.

## 4. Deployment

This section walks through the steps we take to deploy a website. We describe two main methods of deploying to a production server. Always strive for **Method 1.**

1. [  ] Import DB

### Method 1. Git Deployment

1. [  ] make a get **release**.
2. [  ] merge **release** into **master**.

### Method 2. FTP Deployment (with SSH)

1. [  ] zip/archive local site.
2. [  ] ftp zipped archive to remote.
3. [  ] SSH into remote location.
4. [  ] unpack/extract archive.
5. [  ] set permissions.
6. [  ] update configuration (if applicable).
7. [  ] check if its working.
8. [  ] update paths/URLs where applicable.

## 5. Post Deployment

This section walks through the steps we take once the website has been deployed successfully.

1. [  ] execute **Production QA Plan**.
2. [  ] Add **Google Analytics**.
  1. [  ] Add **new property** on google analytics site.
  2. [  ] Add **universal analytics tracking code** to template pages.
3. [  ] Add **Webmaster Tools**.
  1. [  ] Add site to webmaster tools.
  2. [  ] Verify site with google analytics.
  3. [  ] Verify **sitemap.xml**.
  4. [  ] Add **sitemap.xml**.
  5. [  ] Have a cold beer.

## 6. End.
