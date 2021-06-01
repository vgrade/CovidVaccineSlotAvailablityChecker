# Warning
# Not for commercial Purpose, Do not abuse cowin api. Keep request under prescribed limit of 100 calls per IP Address/5 mins
# This is just for educational and personal use purpose. Any kind of harm or loss due to using this script will be solo responsibility of user.
# Developer bear no responsibility for any kind of loss due to using this script.

# How to SetUp
# Open following url in browser to get list of states and pick your state id : https://cdn-api.co-vin.in/api/v2/admin/location/states
# Open following url in browser  after replacing <stateid> with your state id which you got in last step. This will give id of all districts. 
# Pick the district id's where you want to  Search for vaccine. : https://cdn-api.co-vin.in/api/v2/admin/location/districts/<stateid>
# Update the district codes in $DistrictCodes variable 0n line no 20. You can provide multiple district code but load on cowin api will increase.
# Update Minimum Age in #MinAge variable on line no 21
# Update desired vaccine name in $vaccineName variable on line no 22
# Update desired vaccine dose no (eg : 1) on line no 23

# Note
# This will open cowin portal and start beeping loudly where you have to login and book slot manually.
