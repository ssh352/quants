#ͨ��makefile
#���
#����׼��: make config
#����debug�棺make 
#����release�棺
# Ȼ��make -e DEBUG=0
#����release��Ѷ�汾
# make -e DEBUG=0 PRO=E86

include ../public/makefile.define

CPPFLAGS := $(CPPFLAGS) -DUSE_REDIS -I. -I$(APIDIR) -I$(CIFOXDIR) -I$(CIFOXDIR)/mysql -I$(CIFOXDIR)/ctp -I$(CIFOXDIR)/sgit -I$(CIFOXDIR)/hiredis-0.13.3

SRCDIRS := $(SRCDIRS) $(APIDIR) $(APIDIR)/ctphandler $(APIDIR)/fshandler  

INLIBS  := $(INLIBS) $(CIFOXLIBDIR)/libmysqlclient_r.a $(CIFOXLIBDIR)/libjsoncpp_r.a

LDFLAGS := $(LDFLAGS) -L$(CIFOXLIBDIR) -lthostmduserapi -lthosttraderapi -lsgitquotapi -lsgittradeapi -llog4cplus -lhiredis

PROGRAM := $(PROGRAMDIR)/bin/tickmanager

include ../public/makefile.in
