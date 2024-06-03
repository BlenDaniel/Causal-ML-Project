
# Thesis Code and Data Submission for Identifying software project risks using a causal machine learning approach

These are the descriptions of the folders and files included in this folder.  

**1. data_parsing.ipynb  - This notebook contains the data generation steps for running the questions.** 

**2. brave-browser/  - This folder contains the notebooks used for running our experiment on brave-browser, to answer the two questions.** 

**3. vue/  - This folder contains the notebooks used for running our experiment on vue, to answer the two questions.** 

**4. tmp/  - This folder contain the source codes f the repositores by there respective names.** 

**5. data/  - This folder contains the selected two projects datasets and also the generated data.** 

**6. requirments.txt  - Contains the libraries for running the notebooks. Installation guide is written below.** 

## Dataset source

The dataset provided contains data for approximately 200 projects that can be used for fault-proneness, defect prediction, or any other relevant research purposes.

<br>

### Link to github repo
```
https://github.com/grimasta/SERDat/
```

### Link to the original source

[Project Features That Make Machine Learning Based Fault Proneness Analysis Successful](https://figshare.com/articles/dataset/Project_Features_That_Make_Machine-Learning_Based_Fault_Proneness_Analysis_Successful/21044443)



# Set up


## Environment 

1. Create .env
    python3.10 -m venv .env

2. Start the env
    source .env/bin/activate

**Note:** Make sure you have installed `lightgbm` and `graphviz`
#### For Mac only
```
    brew install cmake libomp
```

#### For Mac only
```
    brew install graphviz                                    
    brew info graphviz
    export GRAPHVIZ_DIR="opt/homebrew/Cellar/graphviz/8.0.5"
    pip install pygraphviz --global-option=build_ext --global-option="-I$GRAPHVIZ_DIR/include" --global-option="-L$GRAPHVIZ_DIR/lib"

    pip3 install pygraphviz --global-option=build_ext --global-option="-I$GRAPHVIZ_DIR/include" --global-option="-L$GRAPHVIZ_DIR/lib"
```

3. Install the requirements
```
    pip3 install -r requirements.txt
```
    
4. Make the default enviroment for jupyter `.env`
```    
    ipython kernel install --user --name=.env
```
5. Install NPL file
```
    python3 -m spacy download en_core_web_sm
```
6. Run
```
    jupyter notebook
```
