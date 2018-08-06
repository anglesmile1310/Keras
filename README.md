# Keras document useful.
1.Types model in Keras have two main types:
    a,Sequential model:
          -The Sequential model is a linear stack of layers.
          -Have two ways create a Sequential model:
                   +Via constructor:
                   example:
                            from keras.models import Sequential
                            from keras.layers import Dense, Activation
                            model = Sequential([
                                  Dense(32, input_shape=(784,)),
                                  Activation('relu'),
                                  Dense(10),
                                  Activation('softmax'),
                            ])
                    +Via .add() method:
                    example:
                            model = Sequential()
                            model.add(Dense(32, input_dim=784))
                            model.add(Activation('relu'))
    b,Model class API:
