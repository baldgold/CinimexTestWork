# my_ds_project
#main# - Стартовая точка.

#predict_serv# - Предиктивный сервис -> Разработать сервис, который принимает на вход идентификатор сессии session_id, рассчитывает необходимые параметры для входного вектора модели и возвращает предсказание пола пользователя.

data_serv - Сервис доступа к данным -> Реализовать REST сервис, возвращающий количество просмотров в каждой категории `category` в рамках сессии `session_id`. В зависимости от параметра, возвращать нужно либо относительное количество в процентах от общего, либо абсолютные величины

sqlfile - Написать слой доступа к данным на базе библиотеки SQLAlchemy

model - Необходимо реализовать код для обработки данных и обучения модели предсказания пола пользователя по данным просмотра продукции на сайте. Оформить код нужно в виде Jupyter блокнота. На выходе должен быть отчет по оценки качества работы модели (внутри блокнота) и файл с самой моделью. 
Метрики оценки качества модели и методику тестирования следует проработать самостоятельно.
Не стоит уделять слишком много времени на прототип модели, так как остальные задания являются не менее важными. Необходимо добиться максимум качества в условиях ограниченного времени на реализацию.

  
## Project Organization

```
├── AUTHORS.rst             <- List of developers and maintainers.
├── CHANGELOG.rst           <- Changelog to keep track of new features and fixes.
├── LICENSE.txt             <- License as chosen on the command-line.
├── README.md               <- The top-level README for developers.
├── configs                 <- Directory for configurations of model & application.
├── data
│   ├── external            <- Data from third party sources.
│   ├── interim             <- Intermediate data that has been transformed.
│   ├── processed           <- The final, canonical data sets for modeling.
│   └── raw                 <- The original, immutable data dump.
├── docs                    <- Directory for Sphinx documentation in rst or md.
├── environment.yaml        <- The conda environment file for reproducibility.
├── models                  <- Trained and serialized models, model predictions,
│                              or model summaries.
├── notebooks               <- Jupyter notebooks. Naming convention is a number (for
│                              ordering), the creator's initials and a description,
│                              e.g. `1.0-fw-initial-data-exploration`.
├── references              <- Data dictionaries, manuals, and all other materials.
├── reports                 <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures             <- Generated plots and figures for reports.
├── scripts                 <- Analysis and production scripts which import the
│                              actual PYTHON_PKG, e.g. train_model.
├── setup.cfg               <- Declarative configuration of your project.
├── setup.py                <- Use `python setup.py develop` to install for development or
|                              or create a distribution with `python setup.py bdist_wheel`.
├── src
│   └── my_ds_project       <- Actual Python package where the main functionality goes.
├── tests                   <- Unit tests which can be run with `py.test`.
├── .coveragerc             <- Configuration for coverage reports of unit tests.
├── .isort.cfg              <- Configuration for git hook that sorts imports.
└── .pre-commit-config.yaml <- Configuration of pre-commit git hooks.
```

[conda]: https://docs.conda.io/
[pre-commit]: https://pre-commit.com/
[Jupyter]: https://jupyter.org/
[nbstripout]: https://github.com/kynan/nbstripout
[Google style]: http://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings
[dsproject extension]: https://github.com/pyscaffold/pyscaffoldext-dsproject
