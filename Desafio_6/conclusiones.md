
### Conclusiones:<br />

### Detalle de pruebas realizadas: Se entrenaron 3 modelos con 80 epochs y se probó hacer inferencia con el mismo set de inputs.<br />

*  ### Modelo 1: arquitectura similar a la vista en clase (para el traductor) pero con Embeddings Fasttext<br />
   ### Se observa overfitting, y se obtiene aprox la mitad de respuestas correctas:<br /><br />

    Input: hi <br />
    Response: hello how are you<br />

    Input: how are you?<br />
    Response: i am doing well how are you<br />

    Input: where are you from?<br />
    Response: i am from the united states<br />

    Input: where do you live?<br />
    Response: i like to play video games<br />

    Input: what do you do for a living?<br /> 
    Response: i m a student<br />

    Input: do you have any hobbies?<br />
    Response: i like to read and read<br />

    Input: what do you do for fun?<br />
    Response: i do not like it<br />

    Input: what is your favorite food?<br />
    Response: bred and vegetables<br />

    Input: what do you study?<br />
    Response: degree<br />

    Input: what is your name?<br />
    Response: what is your name<br />

    Input: do you have pets?<br />
    Response: i do not have any<br />

    Input: do you like music?<br />
    Response: do you like<br />

    Input: what is your favorite colour?<br />
    Response: i like to read books<br /><br />

    
*  ### Modelo 2: al Modelo 1 se le agrega una layer de Dropout = 0.4 en el decoder.<br />
   ### En este caso se observa una mejora en los resultados del entrenamiento (mejora el overfitting) y la inferencia muestra un número mayor de respuestas correctas: <br /><br />

    Input: hi<br />
    Response: hello how are you<br />
    
    Input: how are you?<br />
    Response: i am doing well how are you<br />

    Input: where are you from?<br />
    Response: i am from the united states<br />
    
    Input: where do you live?<br />
    Response: i like to play video games<br />

    Input: what do you do for a living?<br />
    Response: i m a student<br />

    Input: do you have any hobbies?<br />
    Response: i like to read<br />

    Input: what do you do for fun?<br />
    Response: i m a student<br />

    Input: what is your favorite food?<br />
    Response: try to guess<br />

    Input: what do you study?<br />
    Response: i am a teacher i like reading<br />

    Input: what is your name?<br />
    Response: i am a teacher i like to read<br />

    Input: do you have pets?<br />
    Response: i do not have any<br />

    Input: do you like music?<br />
    Response: i do i love to read<br />

    Input: what is your favorite colour?<br />
    Response: i like to go to the beach<br /><br />

*  ### Modelo 3: al Modelo 2 se le agrega recurrent_dropout de 0.1 en las layers LSTM del encoder y del decoder (se pasa   como parámetro).<br />
    ### Mejora apenas el problema del overfitting con respecto a lo observado con el Modelo 2. Una diferencia que se aprecia es el tiempo de entrenamiento, que aumenta considerablemente (de 3 seg/epoch para el modelo 2, se incrementa a aprox 70 seg/epoch para el modelo 3). Los resultados son similares a los anteriores aunque aparecen algunas respuestas sin sentido que se repiten para varias preguntas: <br /><br />

    Input: hi<br />
    Response: hello how are you<br />

    Input: how are you?<br />
    Response: i am doing well how are you<br />

    Input: where are you from?<br />
    Response: i am from the united states<br />

    Input: where do you live?<br />
    Response: i like to play video games<br />

    Input: what do you do for a living?<br />
    Response: i m a student<br />

    Input: do you have any hobbies?<br />
    Response: i do i am a student<br />

    Input: what do you do for fun?<br />
    Response: i like to play video games<br />

    Input: what is your favorite food?<br />
    Response: i like to go to the beach<br />

    Input: what do you study?<br />
    Response: i like to play video games<br />

    Input: what is your name?<br />
    Response: i am not sure what you mean<br />

    Input: do you have pets?<br />
    Response: i do not like it<br />

    Input: do you like music?<br />
    Response: i do not like it<br />

    Input: what is your favorite colour?<br />
    Response: i am from the united states<br />
