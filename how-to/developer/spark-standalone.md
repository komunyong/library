# Install Spark standalone on local Ubuntu

## Required

- Ubuntu 16.04
- For Ubuntu 14.04, change all `apt` to `apt-get`

## Process

1. Install java 1.8.0_151 (keep just java 8 to avoid mroe issues in Spark 2.2.0)

```sh
add-apt-repository ppa:webupd8team/java
apt update
apt install oracle-java8-installer
```

2. Install Scala (v.2.11.8)

```sh
apt install scala
```

3. This step is your choices for language usage, Scala or Python (Pyspark)

- **For Scala**: Install sbt, module builder for Scala

```sh
echo "deb https://dl.bintray.com/sbt/debian /" | sudo tee -a /etc/apt/sources.list.d/sbt.list
apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 2EE0EA64E40A89B84B2DF73499E82A75642AC823
apt update
apt install sbt
```

- **For Python**: Spark with Python (Pyspark)

```sh
apt install python3-pip
apt install python3
pip3 install --upgrade pip
pip3 install jupyter
pip3 install py4j
pip3 install pandoc
pip3 install pyspark
pip3 install findspark
```

- **For Python Jupyter Notebook**: Jupyter Notebook with Pyspark

**Note**: Execute `jupyter notebook --no-browser --allow-root`, notebook file will store at current location that Jupyter Notebook got run.

4. Download, extract and install Spark

```sh
wget "http://www-eu.apache.org/dist/spark/spark-2.2.0/spark-2.2.0-bin-hadoop2.7.tgz"
tar -zxvf spark-2.2.0-bin-hadoop2.7.tgz
```

**Note**: you can go to Spark official website and download directly, then extract and install it in your way

5. Export all global vars

```sh
export SPARK_HOME='/mnt/e/Project/spark/spark-2.2.0-bin-hadoop2.7' \
export PATH=$SPARK_HOME:$PATH \
export PYTHONPATH=$SPARK_HOME/python:$PYTHONPATH \
export PYSPARK_DRIVER_PYTHON="jupyter" \
export PYSPARK_DRIVER_PYTHON_OPTS="notebook" \
export PYSPARK_PYTHON=python3
```

6. Change permission of spark folder `chmod -R go+x /mnt/e/Project/spark/spark-2.2.0-bin-hadoop2.7`

7. Test all the thing that you've done

- **For Scala**: Testing for Scala in Spark just execute `spark-shell`

- **For Python**: Testing for Pyspark, just execute `pyspark`

- **For Python Jupyter Notebook**: Testing for Pyspark in Jupyter Notebook

```python
# In notebook
import findspark
findspark.init('[path-to-spark-dir]')
import pyspark
```
