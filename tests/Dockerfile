from alpine:latest
CMD curl -sSL "http://`cat /run/secrets/jenkins_name`:`cat /run/secrets/jenkins_pass`@jenkins/pluginManager/api/xml?depth=1&xpath=/*/*/shortName|/*/*/version&wrapper=plugins" | perl -pe 's/.*?<shortName>([\w-]+).*?<version>([^<]+)()(<\/\w+>)+/\1 \2\n/g'|sed 's/ /:/'

