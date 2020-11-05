# bgal_forma
# hada i5tisar llcod li ktbto mlwale l background
def bgall(pos,bg):
    pos.update()
    clt = pos.winfo_children()
    pos.config(bg=bg)
    my = ttk.Style()
    my.configure('TRadiobutton', background=bg)
    my.configure('TCheckbutton', background=bg)
    for c in clt:
        try:
            c ['bg']=bg
        except:
            pass
        try:
            c ['background']= bg
        except:
            pass
