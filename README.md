# WebIO
## The Java Web Start client application of the BIC-LSU project.

BIC-LSU WebIO transfers data with the [JSch](http://www.jcraft.com/jsch/) SFTP or the Fast Data Transfer ([FDT](http://monalisa.cern.ch/FDT/)).

BIC-LSU WebIO is adapted from the NetBeans [Converter](https://netbeans.org/kb/73/java/javase-jws.html) demo application.

## Command Line Arguments in JNLP File
All arguments should be enclosed in \<application-desc> tags.

**1st Arg**: The IP Address at which the SSH server on the storage server listens.<br />
**2nd Arg**: The port number at which the SSH server on the storage server listens.<br />
**3rd Arg**: The port number at which the FDT server on the storage server listens.<br />
**4th Arg**: The user name on the storage server.<br />
**5th Arg**: The one-time password for the user name in the previous arg on the storage server.<br />
**6th Arg**: The effective duration in minutes of the password in the previous arg on the sotrage server.<br />
**7th Arg**: The directory on the storage server where the data are downloaed from/uploaded to.<br />
**8th Arg**: The operation of this data transmission.  Valid values "download" or "upload".<br />
**9th Arg**: The valid types of local paths.  Valid values "file", "directory", or "both".  This arg helps prevent transferring a directory into a file.<br />
