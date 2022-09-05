# List of Amazon Fire lockscreen ad domains 
## Adding the domains
- - -
Navigate to http://Your-Pihole-IP/admin/groups-domains.php and click on the RegEx filter tab towards the top of the page.

Copy the domains at #(insert link here)# and paste the domains into the box labled as "Domain:" and click Add to Blocklist. 

## Adding more domains
- - -
If ads continue to appear on the lockscreen of your Fire after adding the blocked domains, go to the link http://Your-Pihole-IP/admin/queries.php and identify which domain is serving the ads. Generally the domains tend to be meaningless strings of alphanumeric characters, though it might have amazon somewhere in the list. 
## If a service stops working
- - -
If certain Amazon services stop working, go to the link http://Your-Pihole-IP/admin/queries.php and check which domains are being blocked. Its easiest to find the domains by trying to access the specific service and immediately refreshing the Pi-Hole Query page and whitelisting the domains that show up as blocked. 

Attemping to whitelist one domain at a time and retesting the service is recommended as that'll minimize the chances of accidently unblocking an ad domain. Assuming you can't find the domain at all, simply recopy the RegEx list and paste it into the same box as before, but instead of clicking Add to Blacklist, click Add to Whitelist.
