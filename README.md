 # Cowin vaccine availablity checker
 Powershell script to check cowid vaccine slot availablity in india using public apis of cowin portal

 Warning
 1. Not for commercial usage, Do not abuse cowin api in any circumances as your ip address might get blocked
 2. Keep requests under prescribed limit of 100 calls per IP Address/5 mins.
 3. This is just for educational and personal use purpose. Any kind of harm or loss due to using this script will be solo responsibility of user
 4. Developer bear no responsibility for any kind of loss due to using this script

 How to SetUp
 1. Download the .ps file and edit it using any text editor.
 2. Open following url in browser to get list of states and pick your state id : https://cdn-api.co-vin.in/api/v2/admin/location/states
 3. Open following url in browser  after replacing <stateid> with your state id which you got in last step. This will give id of all districts. 
 4. Pick the district id's where you want to  Search for vaccine. : https://cdn-api.co-vin.in/api/v2/admin/location/districts/<stateid>
 5. Update the district codes in $DistrictCodes variable on line no 2. You can provide multiple district code.
 6. Update Minimum Age in #MinAge variable on line no 3
 7. Update desired vaccine name in $vaccineName variable on line no 5
 8. Update desired vaccine dose no (eg : 1) on line no 5
 9. Optionally update the $MinimumSlotes variable if you are looking for minimum slots more than 1
 9. Now save the script and open Windows powershell and paste the script in it and run. Alternatively, if running external powershell script is enabled on your computer, you can    just double click on the powershell file
 10.Once desired slots are found, this will print the pincode and deails of centers on powershell window, start beeping loudly (provided your computer's audio output is working correctly) and open cowin portal where you have to login and book slot manually. Search for vaccine on pin codes printed on powershell screen

 Note
 1. API responses data from this script is not exactly real time and can be cached data which can be upto 30 minutes old asper cowin api specification. For more details, please refer: https://apisetu.gov.in/public/marketplace/api/cowin/cowin-public-v2
