After cloning the repo, use following commands from the repo directory :-

git clone git@github.com:ambsFlip/allureSamples.git --branch python_sample

pyth3_dir=`which python3`

virtualenv -p $pyth3_dir pyth3

source pyth3/bin/activate

pip3 install -r requirement.txt

python -m pytest --alluredir=allure_pyth_results  test_sample1.py 

allure generate allure_pyth_results/

Deactivate pyth3
