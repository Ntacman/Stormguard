# Stormguard
A repo containing a configuration to use for overcommit, ready to go.

With the current configuration, the configured hooks run in the context of bundle. The brakeman hook also only checks rails apps
by confirming whether there is an app/controllers folder present. Need to add more folders to check for verification of rails app
