- 👋 Hi, I’m @Wrathchyld
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
git remote set-url
<!---
Wrathchyld/Wrathchyld is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
- name: Setup Java JDK
  uses: actions/setup-java@v3.1.0
brew install stripe/stripe-cli/stripe
remote add origin git@github.com:User/UserRepo.git
git remote set-url origin git@github.
actions-runner-linux-x64-2.289.2.tar.gznpm test
```# Create a folder
$ mkdir actions-runner && cd actions-runner# Download the latest runner package
$ curl -o actions-runner-linux-x64-2.289.2.tar.gz -L https://github.com/actions/runner/releases/download/v2.289.2/actions-runner-linux-x64-2.289.2.tar.gz# Optional: Validate the hash
$ echo "7ba89bb75397896a76e98197633c087a9499d4c1db7603f21910e135b0d0a238  actions-runner-linux-x64-2.289.2.tar.gz" | shasum -a 256 -c# Extract the installer
$ tar xzf ./actions-runner-linux-x64-2.289.2.tar.gzuactions-runner-linux-x64-2.289.2.tar.gzhere](./deploy-migrations/README.md)
20201231_

3

Scan to check the

validity of the r
eceipt on Blockchair.comhttps://blockchair.com/bitcoin/transaction/fc3cae3af9df29281f9855ea1d8fe92f7c20d2632cd41d1615a9bc5801b6c0df
get '/callback' do
  # ...
  # Get the access_token using the code sample above
  # ...

  # check if we were granted user:email scope
  scopes = JSON.parse(result)['scope'].split(',')
  has_user_email_scope = scopes.include? 'user:email'
endhttps://github.com/login/oauth/access_tokenget '/callback' do
  # get temporary GitHub code...
  session_code = request.env['rack.request.query_hash']['code']

  # ... and POST it back to GitHub
  result = RestClient.post('https://github.com/login/oauth/access_token',
                          {:client_id => CLIENT_ID,
                           :client_secret => CLIENT_SECRET,
                           :code => session_code},
                           :accept => :json)

  # extract the token and granted scopes
  access_token = JSON.parse(result)['access_token']
end<html>
  <head>
  </head>
  <body>
    <p>
      Well, hello there!
    </p>
    <p>
      We're going to now talk to the GitHub API. Ready?
      <a href="https://github.com/login/oauth/authorize?scope=user:email&client_id=<%= client_id %>">Click here</a> to begin!
    </p>
    <p>
      If that link doesn't work, remember to provide your own <a href="/apps/building-oauth-apps/authorizing-oauth-apps/">Client ID</a>!
    </p>
  </body>
</html>https://github.com/login/oauth/authorize?scope=user:email&client_id=gradle-app.settinghttps://youtrack.jetbrains.com/issue/IDEA-116898-wrapper.properties.gradle
/build/

# Ignore Gradle GUI config
gradle-app.setting

# Avoid ignoring Gradle wrapper jar file (.jar files are usually ignored)
!gradle-wrapper.jar

# Cache of project
.gradletasknamecache

# # Work around https://youtrack.jetbrains.com/issue/IDEA-116898
# gradle/wrapper/gradle-wrapper.properties
Love**is**bold
server.rb

checkout.html

success.html

cancel.html

Download
require 'stripe'
require 'sinatra'

# This is your test secret API key.
Stripe.api_key = 'sk_test_51KlggaISOxj70O5eU3frIqMjtDHErDFCby7esx9qu41fLBSfoMaa9qw6GBO5BZy5TsZWkXQBuGysXSkcmGSjtLLl00OhSvEGn8'

set :static, true
set :port, 4242

YOUR_DOMAIN = 'http://localhost:4242'

post '/create-checkout-session' do
  content_type 'application/json'

  session = Stripe::Checkout::Session.create({
    line_items: [{
      # Provide the exact Price ID (e.g. pr_1234) of the product you want to sell
      price: '{{PRICE_ID}}',
      quantity: 1,
    }],
    mode: 'payment',
    success_url: YOUR_DOMAIN + '/success.html',
    cancel_url: YOUR_DOMAIN + '/cancel.html',
    automatic_tax: {enabled: true},
  })
  redirect session.url, 303
end
jobs:
  build:
    runs-on: ubuntu-20.04
    strategy:
      matrix:
        java: [ '8', '11', '13', '15' ]
    name: Java ${{ matrix.Java }} sample
    steps:
      - uses: actions/checkout@v2
      - name: Setup java
        uses: actions/setup-java@v2
        with:
          distribution: '<distribution>'
          java-version: ${{ matrix.java }}
      - run: java -cp java HelloWorldAppsteps:
- uses: actions/checkout@v2
- uses: actions/setup-java@v2
  with:
    distribution: 'adopt'
    java-version: '11'
    check-latest: true
- run: java -cp java HelloWorldAppmatrix.Javamatrix.java
