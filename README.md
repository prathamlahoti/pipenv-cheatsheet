#### pipenv-cheatsheet

| Operation     | Description |
| ------------- |-------------|
| `pip install pipenv` | Install pipenv on a machine |
| `pipenv --venv` | Check information about initialized venv |
| `pipenv shell` | Activate pipenv |
| `exit` | Disable pipenv |
| `pipenv install` | Generate pipenv based on Pipfile |
| `pipenv install <package_name>` | Install python package |      
| `pipenv install <package_name> --dev` | Install python dev-package |
| `pipenv install -r requirements.txt` | Install python packages from requirements.txt |
| `pipenv install -d` | Install all packages including dev ones |
| `pipenv update` | Update all installed packages |
| `pipenv update -d` | Update all installed packages including dev ones |
| `pipenv uninstall <package_name>` | Delete python package from pipenv |
| `pipenv uninstall --all` | Delete all python packages from pipenv |
| `pipenv graph` | Show packages dependency graph |    
| `pipenv check` | Check for security vulnerabilities and PEP asserts of installed packages |  
| `pipenv lock` | Generate lock file |
| `pipenv lock -r` | Display all installed python packages |
| `pipenv --rm` | Delete installed pipenv |
| `pipenv run <command>` | Execute `command` from pipenv not activating it |

If it needs to change version of python in your pipenv, we could perform it just exchanging the **python_version** in the Pipfile. So then you have to reinitialize your pipenv using  `pipenv --python <typed version>`.

To check whether you need to update your packages in terms of vulnerabilities, type `pipenv check`.
If so, put the appropriate versions of packages in your Pipfile and type `pipenv install` in your command line.

Feel free to create **.env** file within your pipenv. But don't forget to add created one to **.gitignore**
