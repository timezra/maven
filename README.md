timezra's personal Maven repository.
====================================================

snapshots: http://timezra.github.com/maven/snapshots

releases:  http://timezra.github.com/maven/releases

Publishing to gh-pages
----------------------------------------------------
cd /path/to/github/maven/repository/project

git checkout gh-pages

cd /path/to/maven/project

mvn clean deploy -DaltDeploymentRepository=local_maven::default::file:///path/to/github/maven/repository/project/releases

cd /path/to/github/maven/repository/project

git add releases/groupId/artifactId/version

git commit -a -m "Releasing groupId:artifactId:version"

git push



