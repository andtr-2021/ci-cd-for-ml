# CI/CD-for-ML

- Using Continuous Machine Learning to build a CI/CD pipeline for a machine learning application.

Expected Results:

<img width="599" alt="Screenshot 2023-10-24 at 00 49 57" src="https://github.com/andtr-2021/CI-CD-Machine-Learning/assets/79509067/a6fe0ba2-1a10-4da5-9510-b33592a5dc25">


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

`DVC Remote`
- DVC remote is a storage location for DVC files.
- Support different storage types: local, SSH, Amazon S3, Azure, GG Drive. 
- Set up remote: `dvc remote add` | `dvc remote modify` | `dvc remote remove`
- For Amazon S3: `dvc remote add myAWSRemote s3://my-bucket/my-path`
- For local storage: `dvc remote add -d myLocalRemote /path/to/storage`

`DVC Pipeline`
- DVC pipelines are a set of DVC stages that are run sequentially.
- Data versions only are not very useful. 
- Defined in a dvc.yaml file.

<img width="327" alt="Screenshot 2023-10-24 at 10 52 26" src="https://github.com/andtr-2021/ci-cd-for-ml/assets/79509067/615e8b5e-5053-4266-9526-3456d542811e">

`DVC for Hyperparameter Tuning`
- Run `repro` to rerun after changing the hyperparameters.
- Expected Results:

<img width="466" alt="Screenshot 2023-10-24 at 11 21 02" src="https://github.com/andtr-2021/ci-cd-for-ml/assets/79509067/2b437ded-3509-4d9b-85ec-d5594b3f4d94">
