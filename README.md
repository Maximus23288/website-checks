### Node setup

Install the package:
```
yarn global add @website-checks/website-checks
# or
npm i -g @website-checks/website-checks
```

### Docker setup

In [docker-compose.yml], modify the TARGET_URL variable to change the website. 

Then run:
```
docker-compose up
```

## Usage

`website-checks example.com`

### Change output directory
`website-checks example.com --output pdf` would save all PDF files to the local `pdf` directory.

### CLI flags
Currently the following CLI flags will run the matching checks:
```
--check-your-website
--crtsh
--cryptcheck
--hstspreload
--httpobservatory
--lighthouse
--psi
--securityheaders
--ssllabs
--webbkoll
--webhint
--yellowlab
```

For example `website-checks example.com --lighthouse --securityheaders` will run the Lighthouse and Security Headers checks.
