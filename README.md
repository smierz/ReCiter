# ReCiter

## Eclipse Setup
1. Download a zip version of the ReCiter.
2. Create a Java Project in Eclipse named "ReCiter."
3. Unzip the downloaded ReCiter.
4. Copy existing files into ReCiter workspace in Eclipse.
5. Right Click "ReCiter" project in Eclipse.
6. Select "Configure."
7. Select "Convert to Maven Project."
8. Right Click "ReCiter."
9. Select "Build Path."
10. Select "Add Library."
11. Add "JUnit" library.

## MySQL Setup
1. To connect to the VIVO MySQL database.
2. Change the following in *main/database/DbConnectionFactory.java*.
```
	private static final String URL = "jdbc:mysql://localhost/reciter?rewriteBatchedStatements=true";
	private static final String USER = "root";
	private static final String PASSWORD = "";
```
To the following:
```
	private static final String URL = "jdbc:mysql://its-yrkmysqlt01.med.cornell.edu/reciter?rewriteBatchedStatements=true";
	private static final String USER = "reciter_pubs";
	private static final String PASSWORD = password;
```

## XML data setup.
1. Download the xml file *xml.7z*.
2. In Eclipse, create a folder named *data* with 2 inner folders *lucene_index*, *scopus*.
3. Unzip *xml.7z* into *data* as well.

## Running ReCiter
1. To run ReCiter for a specific person.
2. Edit *config.properties*.
3. Run *src/test/examples/pubmed/ReCiterExample.java*.






