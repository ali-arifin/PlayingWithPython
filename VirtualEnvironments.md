# Virtual Environments

Before proceeding, we are going to use the RemoteSigned execution policy to set the permission for the current user that allows the PowerShell to accept downloaded scripts that we trust without making the permissions as broad as they would be with an Unrestricted permission. In the PowerShell, type:

```powershell
Set-ExecutionPolicy -Scope CurrentUser
```

PowerShell will then prompt us to provide an execution policy, and since we want to use RemoteSigned, we’ll type:

```powershell
RemoteSigned
```

We can confirm that this worked by typing:

```powershell
Get-ExecutionPolicy -List
```

## Now let's start with Virtual Environments


Virtual environments enable us to have an isolated space on our computer for Python projects, ensuring that each of our projects can have its own set of dependencies that won’t disrupt any of our other projects.

Each environment is basically a directory in our computer that has a few scripts in it to make it act as an environment.

Once you are in the directory where you would like the environments to live, you can create an environment by running the following command:

```powershell
python -m venv my_env
```

<img width="699" height="115" alt="image" src="https://github.com/user-attachments/assets/7877fa7d-aa4b-4a6d-93e7-4b726db32365" />


The venv module sets up a new directory that contains a few items which we can view with the ls command:

```powershell
ls my_env
```

<img width="697" height="313" alt="image" src="https://github.com/user-attachments/assets/f85c28ba-e8de-4685-a6d7-96a0511baa79" />

These files together work to make sure that your projects are isolated from the broader context of your local machine, so that system files and project files do not mix.


To use this environment, you need to activate it, which you can do by typing the following command that calls the activate script in the Scripts directory:

```powershell
my_env\Scripts\activate
```

<img width="777" height="67" alt="image" src="https://github.com/user-attachments/assets/cb8b7fc2-0170-442c-a4f1-4a8d3d0ecd72" />

Your prompt will now be prefixed with the name of your environment, in this case it is called my_env

To leave the environment, simply type the command deactivate and you will return to your original directory.

<img width="676" height="82" alt="image" src="https://github.com/user-attachments/assets/bf13ac40-3428-4e50-aced-2e9e9054b4ad" />


