# Netflix Movies and TV Shows Data Analysis using SQL  
![Netflix.logo](https://github.com/Mahadevkempe/SQL_Projects/blob/main/Netflix%20Movies%20and%20TV%20Shows/Logo.png)

# Overview

This project involves a comprehensive analysis of Netflix's movies and TV shows data using SQL. The goal is to extract valuable insights and answer various business questions based on the dataset. The following README provides a detailed account of the project's objectives, business problems, solutions, findings, and conclusions.

# Objectives

Analyze the distribution of content types (movies vs TV shows).
Identify the most common ratings for movies and TV shows.
List and analyze content based on release years, countries, and durations.
Explore and categorize content based on specific criteria and keywords.

# Dataset
The data for this project is sourced from the Kaggle dataset:


- [Dataset Link:](https://github.com/Mahadevkempe/SQL_Projects/blob/main/Netflix%20Movies%20and%20TV%20Shows/Netflix.xlsx)

# Schema
CREATE DATABASE netflix;
CREATE TABLE netflix_titles (
    show_id VARCHAR(20),
    type VARCHAR(50),
    title VARCHAR(255),
    director VARCHAR(255),
    cast TEXT,
    country VARCHAR(255),
    date_added VARCHAR(50),
    release_year INT,
    rating VARCHAR(20),
    duration VARCHAR(50),
    listed_in VARCHAR(255),
    description TEXT
);

# Business Problems and Solutions. 

# 1. What is the Total Number of Movies and TV Shows on Netflix?
    SELECT 
          type, COUNT(*)
    FROM
          netflix_titles
    GROUP BY type; 








