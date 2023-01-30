# CI/CD tools

```bash
git clone git@github.com:freeuni-digital-technologies/homework-checker $MODULE_NAME
cd $MODULE_NAME
git-filter-repo --path $MODULE_NAME --path-rename $MODULE_NAME/:''
```

## Adding code coverage
```bash
yarn add --dev nyc istanbul-badges-readme
```

update package.json

```json
{ 
	"scripts: {
		"coverage": "nyc yarn test && rm -r .nyc_output",
	    "make-badges": "istanbul-badges-readme"
	},
	"nyc": {
	    "reporter": [
	      "json-summary"
	    ]
	  }
}

```

add to README.md
```md
###   Coverage
![Statements](#statements#)
![Branches](#branches#)
![Functions](#functions#)
![Lines](#lines#)
```

```bash
gh release create [<tag>]
```

```bash
"files": [
    "src",
    "lib"
  ],
```

```bash
FROM node:latest

WORKDIR /usr/src/app
COPY yarn.lock ./
COPY package.json ./
RUN yarn install --frozen-lockfile
COPY src ./src
COPY tsconfig.json ./
RUN yarn build

ENTRYPOINT ["yarn", "test-submission"]
```

### Creating cli application
package.json
```json
{
	"bin": {
		"$COMMAND_NAME": "$SCRIPT_FILE"
	}
	"build": "tsc && chmod u+x bin/$SCRIPT_FILE"
}
```

testing locally:
[https://github.com/nektos/act][1]


```json
mkdir -p .github/workflows
```

[1]:	https://github.com/nektos/act