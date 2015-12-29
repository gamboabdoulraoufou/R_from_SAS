# R_from_SAS

In this post, i will show how to use R from SAS (on UNIX environment).
The post cover this party:
  - rr

**Prerequisite**  



Go to yout unix console and tape this command to log in R consoleR console
```R
# Go into R console
R

# Make some operations
a = [12]
print(12/a)

```

**Package installation**
```R
# 1- Download R package .tar.gz file for linux and .gzip file for 
install.packages(<pathtopackage>, repos = NULL, type="source")

# Create dir package
mkdir R_packages
cd R_âckages

# Create temp dir to store installation file
mkdir tmp
export TMPDIR=/analytics/farpt/sasprogs/201512_Retention_model/R_packages/tmp
R CMD INSTALL e1071_1.6-8.tar.gz

install.packages("/analytics/farpt/sasprogs/201512_Retention_model/R_packages/e1071_1.6-8.tar.gz", repos = NULL, type="source")
