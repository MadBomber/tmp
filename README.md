# TODOs
- [x] Add Devise
- [x] Add Haml gem
- [x] Create an Item resource
- [x] Remove Item resource
- [x] Remove Item controller
- [x] Implement API authentication
- [ ] Disable session cookies for JSON requests
      - See https://github.com/waiting-for-dev/devise-jwt
- [ ] Figure out what to do with jwt_revocation_strategy
      - See https://dakotaleemartinez.com/tutorials/devise-jwt-api-only-mode-for-authentication/
- [ ] Figure out better cors config https://github.com/cyu/rack-cors
- [ ] Add request specs for registrations, sessions, etc. for API
- [ ] Add authenticated route behaviour shared examples
- [ ] Write request spec for user resourse
- [ ] Add auth helper for request specs
- [ ] Create box model
- [ ] Create message model
- [x] Learn about and use view_component library
- [x] Setup Cuprite
- [x] Write a feature test for logging in
- [x] Write a feature test for logging out
- [x] Write a feature test for Signing up
- [x] Add log out link
- [ ] Setup ActionCable
- [ ] Do something with turbo frames
- [ ] Do something with Stimulus


# Start

## Docker
  - docker-compose up web database redis sidekiq
  - docker-compose exec -it web bash
  - docker-compose exec -it database psql -U postgres

# Application
## Authentication
### Devise
#### Devise and Turbo
##### Session Cookies
At the time of writing this, Devise and turbo streams have some compatability
issues, which can be resolved by disabling turbo in the forms using a HTML data
attribute `data: { turbo: false }`.

There is [an alternative to make turbo work with the devise forms](https://gorails.com/episodes/devise-hotwire-turbo), 
but involves some customizations to devise that are require more advanced
understanding of devise configuration.

##### JWTs
Enpoints that respond to `json` formats are authenticated with JWT tokens.
See also [devise-jwt](https://github.com/waiting-for-dev/devise-jwt)


## View Component
  - https://viewcomponent.org/guide/getting-started.html
## CSS Framework
[Bootstrap](https://getbootstrap.com/docs/5.3/getting-started/introduction/)

# Testing
## System Tests
- [Cuprite](https://github.com/rubycdp/cuprite "cuprite")
  - See also https://evilmartians.com/chronicles/system-of-a-test-setting-up-end-to-end-rails-testing
  - See also https://vtc.hatenablog.com/entry/2022/02/26/175431 (giving cuprite a try using a basic Rack app)
- Docker
  - Uses [browserless' Chrome image](https://www.browserless.io/docs/docker-quickstart)
  - `docker-compose up -d chrome`
  - visit http://localhost:3333/
