# Redmine Restrict Tracker

Restrict root and child trackers to a certain list.

# Install

Clone the plugin and restart redmine
```
git clone git@github.com:sdwolf/redmine_restrict_tracker.git
```

# Configure

Go to Administration > Plugins > Restrict Tracker - Configure.
You will see a list of availabe trackers with their ids.
Configure the parent for each tracker by adding their ids in the text fields,
separated by commas and press Apply.

# Run tests

Make sure you have the testing gems plugin:
```
git clone git@github.com:sdwolf/redmine_testing_gems.git
bundle install
```

Then run
```
rake redmine:plugins:test NAME=r edmine_restrict_tracker
```

To view test coverage go to `plugins/redmine_restrict_tracker/tmp/coverage`
and open `index.html` in a browser