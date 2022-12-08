def gettags = (“git ls-remote -t -h git@github.com:neha06011988/building-a-multibranch-pipeline-project.git”).execute()
return gettags.text.readLines().collect {
it.split()[1].replaceAll(‘refs/heads/’, ”).replaceAll(‘refs/tags/’, ”).replaceAll(“\\^\\{\\}”, ”)
}
