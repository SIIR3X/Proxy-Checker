# Proxy Checker

## Description

This program is designed to test the effectiveness of various proxies by verifying their ability to make requests to a variety of websites. It provides a simple and automated way to identify functional proxies for future use.

## Objective

The main objective of this program is to provide an efficient and organized way to assess the reliability and performance of various proxies across multiple websites. This can be particularly useful for tasks requiring reliable proxies for accessing diverse internet resources.

## Operation

1. **Creation of the 'working_proxies' directory:** A folder designated to store test results is created.
2. **Generation of the 'all_websites.txt' file:** This file, located within the 'working_proxies' directory, lists the proxies that successfully interacted with all tested sites. It serves as a consolidated list of fully operational proxies.
3. **Creation of files per website:** For each tested website, a separate text file is generated in the 'working_proxies' directory. The name of each file corresponds to the URL of the respective site. These files contain proxies capable of sending and receiving requests specifically to the corresponding address.

## Running the Program

The program can be launched from the command prompt on Windows. You need to provide two arguments:

1. **Path to the proxy file:** The first argument should be the full path to the file containing the list of proxies you want to test. Each proxy should be listed on a new line in this file.
2. **Path to the website file:** The second argument is the path to the file listing the websites to test. Each website should be specified on a separate line in the file.

These two files must follow certain conventions.

## Format Conventions

### Proxy File

The file containing proxies must adhere to the following format for each line:

- For proxies without authentication: `ip:port`
- For proxies with authentication: `ip:port:username:password`

### Website File

The file containing the websites to test proxies on must follow the following format for each line:

`url,timeout`  

- url: The URL of the website to test.
- timeout: The maximum timeout (in seconds) to consider a request successful.