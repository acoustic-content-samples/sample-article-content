# sample-article-content

## Watson Content Hub - Article Sample Content

### Summary
The sample-content.zip provided in this repository provides a getting started package of content model artifacts for the IBM Watson Content Hub samples listed below.  The archive contains authoring categories and taxonomy, a content type for authoring articles, image profiles describing different image resolutions, and also includes some sample image assets and article content items.  By following the instructions in the below Deployment section, you can populate your tenant with these sample artifacts, to more quickly and easily get started with the listed samples and learn to develop applications that use Watson Content Hub.

Use this content package with these samples:
+ https://github.com/ibm-wch/sample-article-angular
+ https://github.com/ibm-wch/sample-article-carousel
+ and more...

### Deployment

+ Install the Watson Content Hub Command Line Tools as described here: https://github.com/ibm-wch/wchtools-cli/
+ Download and extract the sample-content.zip archive to a temporary directory.
+ Run the WCH command line tool to push the sample content as follows:

```
  wchtools push -A -v --dir <temporary directory>/sample-content
```

NOTE: The zip archive contains a top level folder called "sample-content", which you must include in the path argument specified to the --dir option.  If you do not specify the full path to the sample-content folder (eg, if you specify the parent temporary directory that you extracted sample-content to), then no artifacts will be pushed to your tenant.   Ensure that the path that you specify to the --dir argument, contains folders named "assets", "categories", "content", "types",  prior to executing the wchtools command.

###Resources

API Explorer reference documentation: https://developer.ibm.com/api/view/id-618

Watson Content Hub developer center: https://developer.ibm.com/wch/

Watson Content Hub forum: https://developer.ibm.com/answers/smartspace/wch/
