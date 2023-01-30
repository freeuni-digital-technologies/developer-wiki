# Development Workflow
## Tools
დააყენე ეს პროგრამები და გაეცანი ინსტრუქციას
- [https://github.com/github/hub][1]

## Creating And Managing Issues
შეხვედრისთვის გამზადებული მექნება ხოლმე მოკლე აღწერები note-ებით, ძირითადად Ready სვეტში.

შეხვედრის დროს/შემდეგ მნიშვნელოვანია შეავსო ნოუთები იმ ინფორმაციით, რომელიც განვიხილეთ. 

**არ დაგავიწყდეს**:
- assign
- add to project board

### მუშაობის პროცესში
- თითოეული issue-ს ბოლოში იყოს Report Heading, სადაც იქნება დაწერილი რა გააკეთე, რა სცადე, რა დრო დახარჯე. 
	- ეს კარგია იმიტომაც რომ ზოგჯერ შეიძლება რაღაც არ გამოგივიდეს მაგრამ ბევრი რამ ისწავლო, და მნიშვნელოვანია ყველას გვგქონდეს overview

## Making Changes
- go to github issue page
- on the right pane, click "create branch"
- checkout the branch locally

## Creating Pull Requests
```bash
hub pull-request -i <N> # <N>-ის მაგივრად issue number
```

## Reviewing Pull Requests
- check out locally
- test
- ask questions via comments
- mark as reviewed once confirmed

[1]:	https://github.com/github/hub