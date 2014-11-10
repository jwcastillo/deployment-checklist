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

1. You are using `git` as version control for all projects.

## 3. Preflight Checks

This section walks through the steps we take **before** deploying any website.

1. [___] Get client hosting information 
2. [___] Go through **QA Checklist**
  1. [___] `Git Merge` to Staging
  2. [___] Note all URLS/paths that will need changing when live ( *the odd static url* )
3. [___] Backup **everything**
  1. [___] Backup **local/dev DB** 
  2. [___] Backup **local/dev site** 
  3. [___] Backup **Remote/existing DB** 
  4. [___] Backup **Remote/existing site** 
4. [___] Develop **Deployment Plan**.
5. [___] Develop **Production QA Plan**.
6. [___] Discuss **Deployment Plan** with key stakeholders.
7. [___] If possible, set live site to maintenance mode.
8. [___] Notify key stakeholders that deployment is in process.

## 4. Deployment

This section walks through the steps we take to deploy a website. We describe two main methods of deploying to a production server. Always strive for **Method 1.**

1. [___] Import **DB**
2. [___] `git branch` to a release (*release/name*)
3. [___] `git merge` to master branch

### Method 1. Git Deployment

TODO

### Method 2. FTP Deployment (with SSH)

1. [___] `zip/archive` local site.
2. [___] `ftp` zipped archive to remote.
3. [___] `SSH` into remote location.
4. [___] `unpack/extract` archive.
5. [___] Set permissions.
6. [___] Update configuration (if applicable).
7. [___] Check if its working.
8. [___] Update paths/URLs where applicable.

## 5. Post Deployment

This section walks through the steps we take once the website has been deployed successfully.

1. [___] execute **Production QA Plan**.
2. [___] Add **Google Analytics**.
  1. [___] Add **new property** on google analytics site.
  2. [___] Add **universal analytics tracking code** to template pages.
3. [___] Add **Webmaster Tools**.
  1. [___] Add site to webmaster tools.
  2. [___] Verify site with google analytics.
  3. [___] Verify **sitemap.xml**.
  4. [___] Add **sitemap.xml**.

## 6. End.

1. [___] Get client sign off.
2. [___] Have a cold beer.
3. [___] Smoke cigar.
4. [___] Repeat 6.2 & 6.3 until you love yourself again.