# RH-Israel-template
This is a [template repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-template-repository) which acts as the skeleton for generating a new repoistory under RH-Israel organization.

oc patch deployment $(params.APP_NAME) -p '{"spec":{"template":{"spec":{"containers":[{"name":"$(params.APP_NAME)","image":"$(params.IMAGE_NAME):$(params.IMAGE_TAG)"}]}}}}'