# bugsnag

URL: https://app.bugsnag.com/testing-73/app2/errors

Before either of these run `yarn install`

### Development
 - yarn run dev
 
### Production Replication
 - yarn run nuxt generate
 - yarn run start

## Issue


First lets prove bugsnag is setup.  start a server and issue this command

`$nuxt.$bugsnag.notify(new Error('this is a client error from console'))`


### Bugsnag events that appear to not work

#### Generate a live error that is not sent
http://localhost:3000/error

Click the "Throw an error" button

#### Generate an error in a client page
http://localhost:3000/error?error=true




