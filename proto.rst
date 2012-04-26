This is what I'd like the interface to look like::
    
    from termy import Termy

    app = Termy(__name__)

    @app.command
    def hello():
        print "Hello world"
    

    @app.command
    def __default__(self):
        print "I override the default command (which lists commands)"

    if __name__ == "__main__":
        app.run()

Running the command (let's just call it app.py)::

    $ app.py

    

Like Flask there should be Blueprint-Like structures to allow for nested
commands.

