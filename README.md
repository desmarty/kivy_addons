# kivy_addons
It is a repository of additional modules for kivy frameworks. All of the work are in alpha stage, but will definitely solve your short term issues.
Do not thank me. :D
Its a responisibility

<pre>
#Change background color of a kivy layout
#Place the CustomGraphics.py file to a folder
#code starts here

import sys
sys.path.append([path to CustomGraphics.py])
from CustomModules import CustomGraphics
from kivy.app import App
from kivy.uix.boxlayout import BoxLayout
from kivy.uix.label import Label

class TestApp(App):
    def build(self):
		layout = BoxLayout(orientation='vertical', size=(Window.width, Window.height))
		label = Label(text="Remember my name: It's Smruti Ranjan Gochhayat")
		layout.add_widget(label)
		CustomGraphics.SetBG(layout, bg_color=[1,0,0,1])
		return layout
if __name__ == '__main__':
	TestApp().run()
	
#code ends here
</pre>
