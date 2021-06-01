 # Cowin vaccine availablity checker
 Powershell script to check cowid vaccine slot availablity in india using public apis of cowin portal

 Warning
 1. Not for commercial usage, Do not abuse cowin api in any circumances as your ip address might get blocked.
 2. Keep requests under prescribed limit of 100 calls per IP Address/5 mins. This is important to understand that abusing cowin api might impact the performance of cowin portal 
    and might attract legal action from govt so  users are advised to use this script sololy on their own descertion.
 3. This is just for educational and personal use purpose. Any kind of harm or loss due to using this script will be solo responsibility of user.
 4. Developer bear no responsibility for any kind of loss due to using this script.

 How to SetUp
 1. Download the .ps file and edity it using any text editor.
 2. Open following url in browser to get list of states and pick your state id : https://cdn-api.co-vin.in/api/v2/admin/location/states
 3. Open following url in browser  after replacing <stateid> with your state id which you got in last step. This will give id of all districts. 
 4. Pick the district id's where you want to  Search for vaccine. : https://cdn-api.co-vin.in/api/v2/admin/location/districts/<stateid>
 5. Update the district codes in $DistrictCodes variable 0n line no 20. You can provide multiple district code but load on cowin api will increase.
 6. Update Minimum Age in MinAge variable on line no 21
 7. Update desired vaccine name in $vaccineName variable on line no 22
 8. Update desired vaccine dose no (eg : 1) on line no 23
 9. Save .ps file and double click to open. 

 Note
 1. This will open cowin portal and start beeping loudly where you have to login and book slot manually.
