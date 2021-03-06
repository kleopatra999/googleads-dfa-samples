# DFA API v1.20 Ruby Samples

This is a collection of samples written in Ruby which provide a starting place
for your experimentation into the DFA API v1.20.

## Prerequisites

Please make sure that you're running Ruby 1.9+ and you've run
`bundle install` on the example directory to install all prerequisites.

## Setup Authentication

These samples use OAuth 2.0 for authentication. Credential information is loaded
from a `dfa_api.yaml` file, which needs to be populated with the following:

 - `username`: your DFA user profile name
 - `client_id`: your OAuth 2.0 client ID
 - `client_secret`: your OAuth 2.0 client secret
 - `refresh_token`: your OAuth 2.0 refresh token
 - `application_name`: a name for your sample application

Learn more about Google APIs and OAuth 2.0 here:

https://developers.google.com/accounts/docs/OAuth2

Or, if you'd like to dive right in, follow these steps.
 - Visit https://console.developers.google.com to register your application.
 - Click on "Credentials" in the left navigation menu
 - Click the button labeled "Create an OAuth2 client ID"
 - Give your application a name and click "Next"
 - Select "Installed Application" as the "Application type"
 - Under "Installed application type" select "Other"
 - Click "Create client ID"
 - Copy the client ID and client secret that were generated into `dfa_api.yaml`
 - Run the `generate_refresh_token.rb` sample, and copy the refresh token into
   `dfa_api.yaml`

## Running the Examples

I'm assuming you've checked out the code and are reading this from a local
directory. If not check out the code to a local directory.

1. Open a sample and fill in any required values (indicated by a variable value
   of "INSERT_*_HERE").

2. Execute the sample, e.g.

        $ ruby create_campaign.rb

3. Examine your shell output, be inspired and start hacking an amazing new app!
