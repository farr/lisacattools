# lisacattools

Python module for interacting with example LISA catalogs

## 1 - Getting Started

These instructions will get you a copy of the project up and running on your local machine, 
either for development and testing purposes or as an installed package.

### 1.1 - Prerequisites

You will need python3 to run this program.

### 1.2 - Installing by cloning the repository

First, we need to clone the repository
```
git clone ...
```

#### 1.2.1 - For users

To install the package for non-root users:
```
make user
```

To install the package on the root system:
```
make
```

#### 1.2.2 - For developers

Create a virtualenv

```
make prepare-dev
source .lisacattools-env
```

Install the sotfware and the external libraries for development purpose

```
make install-dev
```

### 1.3 - Installing by pip

```
pip install lisacattools
```

## 2 - Development (only if the repository has be cloned)

Install the software by PIP (developers version)

Then, develop your code and commit
```
git commit
```
The tests and code style formatter will be run automatically. To ignore the
checks, do
```
git commit --no-verify
```

## 3 - Running the tutorial

Once the software is installed, data must be downloaded for the tutorial. 
The data are downloaded from a google drive and are large files -- ~10GB in total -- and will be installed 
in `tutorial/data`. 
Datasets include a catalog of simulated MBH detections with parameters updated on a weekly cadence, 
and two UCB catalogs, using 3 and 6 months of simulated LISA data.
```
make data
```

Then install jupyter and run the tutorial
```
make demo
```

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

## Authors

* **James I. Thorpe**, **Tyson B. Littenberg** - Initial work
* **Jean-Christophe Malapert**

## License

This project is licensed under the LGPLV3 License - see the [LICENSE](LICENSE) file for details
