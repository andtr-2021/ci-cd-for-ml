# CI-CD-Machine-Learning

- Using Continuous Machine Learning to build a CI/CD pipeline for a machine learning application.

Expected Results:

`SDLC`: Software Development Life Cycle

`SDLC Workflow`:
1. Build: compiling and packaging the code, resolve dependencies.
2. Test: run unit tests, integration tests, and functional tests.
3. Deploy: deploy the application to a test environment.

`CICD for ML`:
- Data Dependency: data versions and management strategy.
- Experiment: Automating hyperparameter tuning.
- Testing: instead of using only unit testings, CICD for ML reuiqres more testing strategies that is used to test the whole data piple. 

`The Process of CICD for ML`:

<img width="1372" alt="Screenshot 2023-10-23 at 22 35 32" src="https://github.com/andtr-2021/CI-CD-Machine-Learning/assets/79509067/9d494378-5f12-4d8a-a763-170b2d28d021">

`Github Actions`: allows to build and automate pipelines directly from the repository.

<img width="958" alt="Screenshot 2023-10-23 at 23 57 23" src="https://github.com/andtr-2021/CI-CD-Machine-Learning/assets/79509067/2a951dd4-8454-4246-9495-9d94f4228ff3">

Github Actions Coomponents:

Events: trigger the workflow to run.
- Push: when a commit is pushed to the repository.
- Pull Request: when a pull request is created.
- Schedule: run the workflow on a schedule.
- Onpening an issue: when an issue is opened.

Workflow: a set of jobs that are run sequentially or in parallel.
- Defined as Yaml files.
- Stored in the .github/workflows directory of the repository.
Jobs: a set of steps that are run sequentially on the same runner.