# sql-pro-ultra-max
10 sql queries to create a table 

-- INIT database
CREATE TABLE inflation_unemployment (
    years VARCHAR(10),
    inflation_rate DECIMAL(5,2),
    unemployment_rate DECIMAL(5,2)
);

INSERT INTO inflation_unemployment (years, inflation_rate, unemployment_rate)
VALUES
    ('2009-10', 10.83, 10.1),
    ('2010-11', 12.11, 10.8),
    ('2011-12', 8.94, 9.8),
    ('2012-13', 7.35, 8.5),
    ('2013-14', 5.98, 8.8),
    ('2014-15', 6.37, 7.3);
    -- QUERY database
SELECT * FROM inflation_unemployment;
SELECT * FROM inflation_unemployment WHERE ProductID = 1;

<img width="626" alt="inflation year wise sql" src="https://github.com/user-attachments/assets/385d2579-0454-4251-ab3f-1a1b2aa5c70c">


-- INIT database
CREATE TABLE startup_companies (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    company_name TEXT NOT NULL,
    established_year INTEGER NOT NULL,
    industry TEXT
);

INSERT INTO startup_companies (company_name, established_year, industry) VALUES
('Ola', 2010, 'Transportation'),
('Zomato', 2008, 'Food Delivery'),
('Paytm', 2010, 'Fintech'),
('Flipkart', 2007, 'E-commerce'),
('Razorpay', 2014, 'Fintech');

-- QUERY database
SELECT * FROM startup_companies;
SELECT * FROM startup_companies WHERE ProductID = 1;

<img width="625" alt="startup companies and year sql" src="https://github.com/user-attachments/assets/ed226bdd-9672-488d-
  8126-ae0ab19a24f1">


  -- INIT database
CREATE TABLE school_classes (
    class_id INTEGER PRIMARY KEY AUTOINCREMENT,
    class_name TEXT NOT NULL,
    number_of_students INTEGER NOT NULL
);

INSERT INTO school_classes (class_name, number_of_students) VALUES
('Class 1', 30),
('Class 2', 28),
('Class 3', 25),
('Class 4', 32),
('Class 5', 29);

-- QUERY database
SELECT * FROM school_classes;
SELECT * FROM school_classes WHERE ProductID = 1;

<img width="634" alt="class and no  of students sql" src="https://github.com/user-attachments/assets/eb3dc656-a3dd-41d8-a668-459d0032acc6">


-- INIT database
CREATE TABLE crime_scene_report (
    date INTEGER,
    type TEXT,
    description TEXT,
    city TEXT
);

INSERT INTO crime_scene_report (date, type, description, city) VALUES
(20220115, 'burglary', 'Residential burglary reported in the neighborhood.', 'Springfield'),
(20220116, 'assault', 'Individual assaulted near downtown.', 'Springfield'),
(20220117, 'theft', 'Shoplifting incident at local grocery store.', 'Springfield'),
(20220118, 'murder', 'Body found in abandoned warehouse.', 'Springfield'),
(20220119, 'vandalism', 'Graffiti reported on school property.', 'Springfield');

-- QUERY database
SELECT * FROM crime_scene_report;
SELECT * FROM crime_scene_report WHERE ProductID = 1;

<img width="641" alt="crime scene report sql" src="https://github.com/user-attachments/assets/2d855a2d-7939-400f-b151-df9bb6f933d9">


-- INIT database
CREATE TABLE countries_population (
    country_name TEXT PRIMARY KEY,
    female_population INTEGER,
    male_population INTEGER,
    total_population INTEGER
);

INSERT INTO countries_population (country_name, female_population, male_population, total_population) VALUES
('India', 662000000, 694000000, 1356000000),
('United States', 167000000, 162000000, 329000000),
('Brazil', 105000000, 100000000, 205000000),
('Nigeria', 101000000, 102000000, 203000000),
('Germany', 42000000, 41000000, 83000000);

-- QUERY database
SELECT * FROM countries_population;
SELECT * FROM countries_population WHERE ProductID = 1;

<img width="640" alt="country and populations sql" src="https://github.com/user-attachments/assets/cbb3746a-c03b-46df-87d1-da53685c32eb">


-- INIT database
CREATE TABLE monthly_sales (
    sales_id INTEGER PRIMARY KEY AUTOINCREMENT,
    month TEXT NOT NULL,
    year INTEGER NOT NULL,
    total_sales DECIMAL(10, 2) NOT NULL,
    total_units_sold INTEGER NOT NULL
);

INSERT INTO monthly_sales (month, year, total_sales, total_units_sold) VALUES
('January', 2023, 15000.00, 200),
('February', 2023, 17000.00, 250),
('March', 2023, 16000.00, 230),
('April', 2023, 18000.00, 300),
('May', 2023, 20000.00, 350);

-- QUERY database
SELECT * FROM monthly_sales;
SELECT * FROM monthly_sales WHERE ProductID = 1;

<img width="636" alt="company and sales sql" src="https://github.com/user-attachments/assets/2382d0f6-e022-4119-817b-d85df6c44823">


-- INIT database
CREATE TABLE india_population (
    year INTEGER PRIMARY KEY,
    population INTEGER NOT NULL
);


INSERT INTO india_population (year, population) VALUES
(1991, 846387888),
(2001, 1028700000),
(2011, 1210193422);

-- QUERY database
SELECT * FROM india_population;
SELECT * FROM india_population WHERE ProductID = 1;

<img width="641" alt="india 3 years population sql" src="https://github.com/user-attachments/assets/947946c5-295c-4289-924b-921f52a61eba">


-- INIT database
CREATE TABLE library_books (
    book_id INTEGER PRIMARY KEY AUTOINCREMENT,
    title TEXT NOT NULL,
    author TEXT NOT NULL,
    publication_year INTEGER,
    genre TEXT,
    available_copies INTEGER NOT NULL
);


INSERT INTO library_books (title, author, publication_year, genre, available_copies) VALUES
('To Kill a Mockingbird', 'Harper Lee', 1960, 'Fiction', 3),
('1984', 'George Orwell', 1949, 'Dystopian', 5),
('Pride and Prejudice', 'Jane Austen', 1813, 'Romance', 2),
('The Great Gatsby', 'F. Scott Fitzgerald', 1925, 'Fiction', 4),
('Moby Dick', 'Herman Melville', 1851, 'Adventure', 1);

-- QUERY database
SELECT * FROM library_books;
SELECT * FROM library_books WHERE ProductID = 1;

<img width="641" alt="library books sql" src="https://github.com/user-attachments/assets/1635d208-4ffe-40f4-8b36-c4c29967b73b">


-- INIT database
CREATE TABLE instagram_insights (
    month TEXT PRIMARY KEY,
    followers INTEGER NOT NULL,
    impressions INTEGER NOT NULL,
    engagement_rate DECIMAL(5, 2) NOT NULL,
    profile_visits INTEGER NOT NULL
);


INSERT INTO instagram_insights (month, followers, impressions, engagement_rate, profile_visits) VALUES
('01', 1200, 15000, 5.25, 300),
('02', 1300, 18000, 6.00, 400),
('03', 1350, 16000, 5.75, 350),
('04', 1400, 20000, 6.50, 450),
('05', 1450, 22000, 7.00, 500),
('06', 1500, 25000, 7.50, 600);

-- QUERY database
SELECT * FROM instagram_insights;
SELECT * FROM instagram_insights WHERE ProductID = 1;

<img width="656" alt="insta insights sql" src="https://github.com/user-attachments/assets/28f9aa2a-9d4a-441e-911c-3129e88600d6">


-- INIT database
CREATE TABLE hdi_ranking (
    country_id INT PRIMARY KEY,
    country_name VARCHAR(100) NOT NULL,
    hdi_score DECIMAL(3, 2) NOT NULL,
    rank INT NOT NULL
);


INSERT INTO hdi_ranking (country_id, country_name, hdi_score, rank) VALUES
(1, 'Norway', 0.961, 1),
(2, 'Switzerland', 0.955, 2),
(3, 'Ireland', 0.955, 3),
(4, 'Germany', 0.947, 4),
(5, 'Australia', 0.955, 5);

-- QUERY database
SELECT * FROM hdi_ranking;
SELECT * FROM hdi_ranking WHERE ProductID = 1;

<img width="635" alt="hdi ranking sql" src="https://github.com/user-attachments/assets/0f2e67c2-c582-4744-afbf-a3f45d5b4a0c">
