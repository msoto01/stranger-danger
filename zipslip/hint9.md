# Hint 9

```java
1.   	final String canonicalDestinationDirPath = new File("/* <your destination dir> */").getCanonicalPath();
2.    	ZipFile zip = new ZipFile("/* <your zip file> */");
3.    	Enumeration<ZipEntry> entries =  (Enumeration<ZipEntry>) zip.entries();
4.    	while (entries.hasMoreElements()) {
5.    	  ZipEntry e = entries.nextElement();
6.    	  File f = new File(canonicalDestinationDirPath, e.getName());
7.    	  String canonicalDestinationFile = f.getCanonicalPath();
8.    	  	    	  
9.    	  if (!canonicalDestinationFile.startsWith(canonicalDestinationDirPath + File.separator)) {
10.   		throw new Exception("Entry is outside of the target dir: " + e.getName());
11.   	  }
12.	  
13.   	  InputStream input = zip.getInputStream(e);
14.   	  FileUtils.copyToFile(input, f);
15.   	}
```
