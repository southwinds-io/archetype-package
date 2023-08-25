# Artisan Package Archetype

Use this archetype as the basis to build a new package.
The archetype can be built and shows the basic structure of a fully functional package.
Note that you can define your own structure, this archetype is one possible layout for a package project,
and it is offered as a good practice example.

> *Change the code inside to suit your needs. Know you can use any tools or automation you want.
Comments have been added to the code explaining the key concepts.
Artisan is just a vehicle to ship your logic in a standard, secure and edge friendly way.*

## Building the package

### Clone the repository

```bash
$ git clone https://github.com/southwinds-io/archetype-package <project-name>
```

### Building the package

To build the package type the following command from within the root folder:

```bash
$ art build -t localhost:8082/test/archetype:1.0 -p default .
```

> *The command above is saying:
build me a package called `localhost:8082/test/archetype:1.0` using the `default` build profile that is located in 
the current folder's `.` build file*

If you know docker, artisan works in a similar way, in regard to tagging, pulling, pushing and building operations.

### Listing the package

To see the package that has just been built run the following command:

```bash
$ art ls
```

### Listing the package API

To see the package API run the following command:

``` bash
$ art man fx localhost:8082/test/archetype:1.0
```

### Running functions on the package

