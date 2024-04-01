1. Start Minio by executing the provided `docker-compose.mino.yml` file, or choose an alternative method to initiate Minio.

2. Once Minio is operational, within its interface, create a bucket titled "data" and generate access and secret keys for your use.

3. All code implementations must be completed within the assigned files: `download.ipynb` and `transform.ipynb`.

4. Employ Selenium to automate the download of a file accessible via the specified Google Drive link provided in `download.ipynb`.

5. Unzip the downloaded .zip file and proceed to upload all contained files to the "data-raw" directory within the Minio bucket created earlier.

6. Utilize Spark to establish a connection with Minio and read the stored data. Useful hints for this task are available in the `transform.ipynb` file.

7. Utilize Spark to merge three JSON files (`data.json`, `data2.json`, and `data3.json`) into a single file named `result.json`. Subsequently, upload the merged file to the "data-result" directory in Minio.

8. Read the contents of the `result.json` file using Spark, display the data, remove any duplicate entries, and display the processed data again. Ensure to maintain a record of the crucial steps undertaken during this process.

9. Evaluate the results: Confirm whether the number of records decreases from 19 to 18 after the removal of duplicates. Additionally, ascertain if the final outcome is a CSV file successfully uploaded to Minio, and verify its readability.
