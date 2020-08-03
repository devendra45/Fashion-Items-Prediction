## Usage

### Loading data with Python (requires NumPy)

  Use utils/mnist_reader in this repo:

  import mnist_reader
  
  X_train, y_train = mnist_reader.load_mnist('data/fashion', kind='train')

  X_test, y_test = mnist_reader.load_mnist('data/fashion', kind='t10k')

-------------------------------------------------------------------------------------------------------------------------------------

### Loading data with Tensorflow

  Make sure you have downloaded the data and placed it in data/fashion. Otherwise, Tensorflow will download and use the original MNIST.

  from tensorflow.examples.tutorials.mnist import input_data

  data = input_data.read_data_sets('data/fashion')

  data.train.next_batch(BATCH_SIZE)
