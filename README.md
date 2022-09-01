# QAssist



## How To Use

You can use [Google Colab](https://colab.research.google.com/) to run the jupyter notebook we provide here.

At the beginning of each notebook, there are a set of commands to install the required libraries and prepare the environment.

The replication notebooks require the objects within the *replication* folder. So if you end up using Colab, you will need to [upload them your environment](https://neptune.ai/blog/google-colab-dealing-with-files)


### QG_component notebook

After Installing the required libraries by running the first four cells, runtime restart is required (5th cell). 

Once a runtime restart is done, you can go ahead and run the rest of the notebook (Do not rerun the installation commands cells 1-4 again).

### Replication/IR_notebook

For the IR notebook, you can put the connect the environment with your Google Drive, if not you can remove the last two lines from the second cell.
This notebook requires **GTv6.obj** and **dexV2.obj** to run, which are found in the *replication* folder. 
Adjust the path to these objects when loading them in cell 5 and 12.

The results of each step are saved in the *results* dictionnary object which you can call anytime to see the saved results.

At the end of the notebook, the *results* object can be visualized as a Pandas table.

### Replication/MRC_notebook

Similar to the IR notebook, you connect to Google Drive, or remove the last two line of the second cell. 
This notebook requires **GTv6.obj** to run, which can be found in the *replication* folder. 
Adjust the path to this object when loading it in cell 5.

This notebook runs an ElasticSearch server, this server may stop for various reasons. 
When this happens a *ConnectionError* is raised. If you encounter this error, you can solve it by restarting the Elastic server (cell 15).

## License

This project is open-source under MIT license
