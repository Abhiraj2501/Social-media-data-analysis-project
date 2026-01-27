Exploratory Recommendation Systems Analysis
Overview

This project focuses on exploratory analysis for building interpretable recommendation systems by studying user–entity relationships and interaction patterns. The objective is not to train a black-box recommender, but to understand the data, extract meaningful features, and validate decision logic through structured analysis.

The dataset consists of semi-structured profile-level data, which is parsed, cleaned, and transformed into a structured JSON format for downstream analysis.
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Objectives

Convert semi-structured textual data into a structured dataset

Analyze user-level attributes such as posts, followers, and following counts

Identify influential entities and behavioral patterns

Support feature-driven recommendation logic through exploratory insights

Emphasize interpretability and decision validation over blind prediction
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Dataset Description

The raw data is stored as a text file where each user profile is separated by blank lines. Each profile includes:

Username

Number of posts

Followers count (supports K / M notation)

Following count (supports K / M notation)

Display name

Page type / category

Bio or description text

Data Processing Pipeline
1. Data Ingestion

Reads raw text data using UTF-8 encoding

Splits data into individual user profile chunks

2. Parsing & Cleaning

Extracts numerical fields and normalizes follower/following counts

Handles missing or unknown page categories

Preserves unstructured bio text for future NLP-based analysis

3. Structuring

Converts parsed data into a list of dictionaries

Exports the cleaned dataset into a JSON file (data.json)

4. Exploratory Analysis

Identifies:

User with maximum posts

User with maximum followers

User with maximum followings

Extracts and counts unique page categories
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
