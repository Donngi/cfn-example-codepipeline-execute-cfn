deploy-with-local:
	rain deploy cfn-execution-pipeline.yaml \
		-c config/local.yaml \
		--params BuildSpecCi='$(shell cat buildspec/buildspec-ci.yml)'  \
		--params BuildSpecCreateChangeSet='$(shell cat buildspec/buildspec-create-change-set.yml)' \
		--params BuildSpecDeploy='$(shell cat buildspec/buildspec-deploy.yml)' \
		-y

deploy-with-dev:
	rain deploy cfn-execution-pipeline.yaml \
		-c config/dev.yaml \
		--params BuildSpecCi='$(shell cat buildspec/buildspec-ci.yml)' \
		--params BuildSpecCreateChangeSet='$(shell cat buildspec/buildspec-create-change-set.yml)' \
		--params BuildSpecDeploy='$(shell cat buildspec/buildspec-deploy.yml)' \
		-y
