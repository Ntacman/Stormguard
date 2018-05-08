# Stormguard
A repo containing a configuration to use for overcommit, ready to go.

With the current configuration, the configured hooks run in the context of bundle. The brakeman hook also only checks rails apps
by confirming whether there is an app/controllers folder present. Need to add more folders to check for verification of rails app

Steps to set up overcommit
1. `gem install overcommit`
1. Install any of the gems used in the hooks, in this case, `rubocop`, `brakeman`, `fasterer`, `reek`, and `rubocop`
1. drop the `.overcommit.yml` file into the root of your git repo
1. `run overcommit --install`

Note: you can also configure git to automatically install the hook in all future git repos by configuring
GIT_TEMPLATE_DIR in your shell. I have yet to configure this, will add instructions after testing
