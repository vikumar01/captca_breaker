# captca_breaker

Implemented used keras

#Generating captchas
./generate.py --width 128 --height 64 --length 4 --symbols symbols.txt --count 3200 --output-dir test


Training the neural network
./train.py --width 128 --height 64 --length 4 --symbols symbols.txt --batch-size 4 --epochs 2 --output-model test.h5 --train-dataset 

Running the classifier
./classify.py  --model-name test --captcha-dir ~/Downloads/validation_data/ --output ~/Downloads/stuff.txt --symbols symbols.txt
