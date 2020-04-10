'''
Fixed And Builded By Uwewww
Special Thanks To Cipul
Supported By:
	Dolphin
	Aditmadzs
	Rynkings
	Tanysyz
	Justferians.us
	Muhmursalind
	Aditya Nugraha
	Fathan
	Rhyn
	Agee
	Khie
	Yehezkiel Bagas
	Gio Mahendra
	Grimm
	ᴛᴇᴀᴍ ᴇʟɪᴛᴇ ʙᴏᴛ
	HelloWorld Square
©2019 By Sentinel™
'''
from sentinel import *
from akad.ttypes import *
from time import sleep
from threading import Thread
import pytz, datetime, time, timeit, livejson, asyncio, random, sys, ast, re, os, json, subprocess, threading, string, codecs, requests, ctypes, urllib,traceback,platform
from datetime import timedelta, date
from datetime import datetime
#Sentinel™
#Login Option Below
#Email : LINE("email","Password")
#Auth Token : LINE("authtoken")
#Primary Token : LINE("primary",appName='IOS 8.16.1 Iphone7')
programStart = time.time()
cl = LINE()
print('==== UNIT 1 READY ! ====')
ki = LINE()
print('==== UNIT 2 READY ! ====')
kk = LINE()
print('==== UNIT 3 READY ! ====')
kc = LINE()
print('==== UNIT 4 READY ! ====')
kd = LINE()
print('==== UNIT 5 READY ! ====')
ke = LINE()
print('==== UNIT 6 READY ! ====')
a1 = LINE()
print('==== UNIT 7 READY ! ====')
a2 = LINE()
print('==== UNIT 8 READY ! ====')
a3 = LINE()
print('==== UNIT 9 READY ! ====')
sw = LINE()
print('==== UNIT 10 READY ! ====')

print ('ALL UNIT READY !')

oepoll = OEPoll(cl)
myMid = cl.profile.mid
mid = cl.getProfile().mid
Amid = ki.getProfile().mid
Bmid = kk.getProfile().mid
Cmid = kc.getProfile().mid
Dmid = kd.getProfile().mid
Emid = ke.getProfile().mid
Fmid = a1.getProfile().mid
Gmid = a2.getProfile().mid
Hmid = a3.getProfile().mid
Zmid = sw.getProfile().mid
KAC = [cl,ki,kk,kc,kd,ke,a1,a2,a3,sw]
ABC = [ki,kk,kc,kd,ke,a1,a2,a3,sw]

event_loop = asyncio.get_event_loop()
status = livejson.File('status.json', True, False, 4)
ban = livejson.File('blacklist.json', True, False, 4)
with open("settings.json","r",encoding="utf-8") as fp:
	settings = json.load(fp)
Uwewbots = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid,Zmid,"u38149c6501e323712f8ab24276fcd65f","u77056f10624fd702a155b84d7dfe39b0","u5300d76c46ce56890db3bbee44bcf376","u4fe7c05c855bd242fd43120cae10a121","u6a300cbfebf8eb5e3ce900091f73f3ac","ub3cd981a8c92398cb939854602929d99","u5ccb2bd0df5684f14f64d7abaadd2589","u3a936c6e111bb1c95b6fd67f8599d4c8","u00d949dd841897a10e3f3824a320650b","u488f19e5d5f3d843991c5b863e2edf10","u734f29aae0e572a358d9e499ade73639","u8bb5a06bb4420b91b1b7d7a47450e26b","u1eedd8a03bee09b3bd7df0a3b4bab51c","u24f4eb1c573fffd80008c1f4053d9980"]
creator = status["creator"] #Insert Creator Mid In Settings.json
cerberusowner = status["owner"] #Insert Owner Mid In Settings.json
cerberusadmin = status["admin"] #Insert Admin Mid In Settings.json Or You Can Add When Bots Runs
cerberusstaff = status["staff"] #Insert Staff Mid In Settings.json Or You Can Add When Bots Runs
cerberusbots = status["Bots"] #Insert Bots Mid In Settings.json Or You Can Add When Bots Runs
owner = status["owner"] and cerberusowner
admin = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid,Zmid] and cerberusadmin
staff = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid,Zmid] and cerberusstaff
Bots = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid,Zmid] and cerberusbots
Cerberus = creator and owner and admin and staff and Bots
Team = [ki,kk,kc,kd,ke,a1,a2,a3]
Squad = [cl,ki,kk,kc,kd,ke,a1,a2,a3,sw]
Uwewlist = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid,Zmid,"ud5b11bf786ffbabd45a7a83157e3fbcc"]

sname1 = cl.getProfile().displayName
sname2 = ki.getProfile().displayName
sname3 = kk.getProfile().displayName
sname4 = kc.getProfile().displayName
sname5 = kd.getProfile().displayName
sname6 = ke.getProfile().displayName
sname7 = a1.getProfile().displayName
sname8 = a2.getProfile().displayName
sname9 = a3.getProfile().displayName

read = {
    "ROM": {},
    "readPoint": {},
    "readMember": {},
    "readTime": {},
}

cctv = {
    "cyduk":{},
    "point":{},
    "sidermem":{}
}


tz = pytz.timezone("Asia/Jakarta")
timeNow = datetime.now(tz=tz)

for uwew in Squad:
	for uwewww in Uwewlist:
		try:
			uwew.findAndAddContactsByMid(uwewww)
		except:
			pass

def restart_program():
	print('####==== PROGRAM RESTARTED ====####')
	backupData()
	python = sys.executable
	os.execl(python, python, * sys.argv)
def restartBot():
	print('####==== PROGRAM RESTARTED ====####')
	backupData()
	python = sys.executable
	os.execl(python, python, * sys.argv)

def bckqrprot(grup):
	try:
		G = cl.getGroup(grup)
		G.preventedJoinByTicket = False
		cl.updateGroup(G)
		Ridwan = cl.reissueGroupTicket(grup)
		a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
		for u in a:
			u.acceptGroupInvitationByTicket(grup,Ridwan)
		G = cl.getGroup(grup)
		G.preventedJoinByTicket = True
		cl.updateGroup(G)
	except:
		try:
			G = ki.getGroup(grup)
			G.preventedJoinByTicket = False
			ki.updateGroup(G)
			Ridwan = ki.reissueGroupTicket(grup)
			a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
			for u in a:
				u.acceptGroupInvitationByTicket(grup,Ridwan)
			G = ki.getGroup(grup)
			G.preventedJoinByTicket = True
			ki.updateGroup(G)
		except:
			try:
				G = kk.getGroup(grup)
				G.preventedJoinByTicket = False
				kk.updateGroup(G)
				Ridwan = kk.reissueGroupTicket(grup)
				a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
				for u in a:
					u.acceptGroupInvitationByTicket(grup,Ridwan)
				G = kk.getGroup(grup)
				G.preventedJoinByTicket = True
				kk.updateGroup(G)
			except:
				try:
					G = kc.getGroup(grup)
					G.preventedJoinByTicket = False
					kc.updateGroup(G)
					Ridwan = kc.reissueGroupTicket(grup)
					a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
					for u in a:
						u.acceptGroupInvitationByTicket(grup,Ridwan)
					G = kc.getGroup(grup)
					G.preventedJoinByTicket = True
					kc.updateGroup(G)
				except:
					try:
						G = kd.getGroup(G)
						G.preventedJoinByTicket = False
						kd.updateGroup(G)
						Ridwan = kd.reissueGroupTicket(grup)
						a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
						for u in a:
							u.acceptGroupInvitationByTicket(grup,Ridwan)
						G = kd.getGroup(grup)
						G.preventedJoinByTicket = True
						kd.updateGroup(G)
					except:
						try:
							G = ke.getGroup(grup)
							G.preventedJoinByTicket = False
							ke.updateGroup(G)
							Ridwan = ke.reissueGroupTicket(grup)
							a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
							for u in a:
								u.acceptGroupInvitationByTicket(grup,Ridwan)
							G = ke.getGroup(grup)
							G.preventedJoinByTicket = True
							ke.updateGroup(G)
						except:
							try:
								G = a1.getGroup(grup)
								G.preventedJoinByTicket = False
								a1.updateGroup(G)
								Ridwan = a1.reissueGroupTicket(grup)
								a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
								for u in a:
									u.acceptGroupInvitationByTicket(grup,Ridwan)
								G = a1.getGroup(grup)
								G.preventedJoinByTicket = True
								a1.updateGroup(G)
							except:
								try:
									G = a2.getGroup(grup)
									G.preventedJoinByTicket = False
									a2.updateGroup(G)
									Ridwan = a2.reissueGroupTicket(grup)
									a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
									for u in a:
										u.acceptGroupInvitationByTicket(grup,Ridwan)
									G = a2.getGroup(grup)
									G.preventedJoinByTicket = True
									a2.updateGroup(G)
								except:
									try:
										G = a3.getGroup(grup)
										G.preventedJoinByTicket = False
										a3.updateGroup(G)
										Ridwan = a3.reissueGroupTicket(grup)
										a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
										for u in a:
											u.acceptGroupInvitationByTicket(grup,Ridwan)
										G = a3.getGroup(grup)
										G.preventedJoinByTicket = True
										a3.updateGroup(G)
									except:
										pass

def antijs(grup, target):
	try:
		sw.acceptGroupInvitation(grup)
		sw.kickoutFromGroup(grup, [target])
		sw.leaveGroup(grup)
		cl.inviteIntoGroup(grup, [Zmid])
	except:
		try:
			sw.acceptGroupInvitation(grup)
			sw.kickoutFromGroup(grup, [target])
			sw.leaveGroup(grup)
			ki.inviteIntoGroup(grup, [Zmid])
		except:
			try:
				sw.acceptGroupInvitation(grup)
				sw.kickoutFromGroup(grup, [target])
				sw.leaveGroup(grup)
				kk.inviteIntoGroup(grup, [Zmid])
			except:
				try:
					sw.acceptGroupInvitation(grup)
					sw.kickoutFromGroup(grup, [target])
					sw.leaveGroup(grup)
					kc.inviteIntoGroup(grup, [Zmid])
				except:
					try:
						sw.acceptGroupInvitation(grup)
						sw.kickoutFromGroup(grup, [target])
						sw.leaveGroup(grup)
						kd.inviteIntoGroup(grup, [Zmid])
					except:
						try:
							sw.acceptGroupInvitation(grup)
							sw.kickoutFromGroup(grup, [target])
							sw.leaveGroup(grup)
							ke.inviteIntoGroup(grup, [Zmid])
						except:
							try:
								sw.acceptGroupInvitation(grup)
								sw.kickoutFromGroup(grup, [target])
								sw.leaveGroup(grup)
								a1.inviteIntoGroup(grup, [Zmid])
							except:
								try:
									sw.acceptGroupInvitation(grup)
									sw.kickoutFromGroup(grup, [target])
									sw.leaveGroup(grup)
									a2.inviteIntoGroup(grup, [Zmid])
								except:
									try:
										sw.acceptGroupInvitation(grup)
										sw.kickoutFromGroup(grup, [target])
										sw.leaveGroup(grup)
										a3.inviteIntoGroup(grup, [Zmid])
									except:
										pass

def antijs3(grup,target):
	try:
		cl.inviteIntoGroup(grup, [Zmid])
		sw.acceptGroupInvitation(grup)
		sw.kickoutFromGroup(grup, [target])
		itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
		sw.inviteIntoGroup(grup, itu)
		sw.leaveGroup(grup)
	except:
		try:
			ki.inviteIntoGroup(grup, [Zmid])
			sw.acceptGroupInvitation(grup)
			sw.kickoutFromGroup(grup, [target])
			itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
			sw.inviteIntoGroup(grup, itu)
			sw.leaveGroup(grup)
		except:
			try:
				kk.inviteIntoGroup(grup, [Zmid])
				sw.acceptGroupInvitation(grup)
				sw.kickoutFromGroup(grup, [target])
				itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
				sw.inviteIntoGroup(grup, itu)
				sw.leaveGroup(grup)
			except:
				try:
					kc.inviteIntoGroup(grup, [Zmid])
					sw.acceptGroupInvitation(grup)
					sw.kickoutFromGroup(grup, [target])
					itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
					sw.inviteIntoGroup(grup, itu)
					sw.leaveGroup(grup)
				except:
					try:
						kd.inviteIntoGroup(grup, [Zmid])
						sw.acceptGroupInvitation(grup)
						sw.kickoutFromGroup(grup, [target])
						itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
						sw.inviteIntoGroup(grup, itu)
						sw.leaveGroup(grup)
					except:
						try:
							ke.inviteIntoGroup(grup, [Zmid])
							sw.acceptGroupInvitation(grup)
							sw.kickoutFromGroup(grup, [target])
							itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
							sw.inviteIntoGroup(grup, itu)
							sw.leaveGroup(grup)
						except:
							try:
								a1.inviteIntoGroup(grup, [Zmid])
								sw.acceptGroupInvitation(grup)
								sw.kickoutFromGroup(grup, [target])
								itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
								sw.inviteIntoGroup(grup, itu)
								sw.leaveGroup(grup)
							except:
								try:
									a2.inviteIntoGroup(grup, [Zmid])
									sw.acceptGroupInvitation(grup)
									sw.kickoutFromGroup(grup, [target])
									itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
									sw.inviteIntoGroup(grup, itu)
									sw.leaveGroup(grup)
								except:
									try:
										a3.inviteIntoGroup(grup, [Zmid])
										sw.acceptGroupInvitation(grup)
										sw.kickoutFromGroup(grup, [target])
										itu = [mid,Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
										sw.inviteIntoGroup(grup, itu)
										sw.leaveGroup(grup)
									except:
										pass

def qrprot(grup):
	try:
		G = cl.getGroup(grup)
		G.preventedJoinByTicket = True
		cl.updateGroup(G)
	except:
		try:
			G = ki.getGroup(grup)
			G.preventedJoinByTicket = True
			ki.updateGroup(G)
		except:
			try:
				G = kk.getGroup(grup)
				G.preventedJoinByTicket = True
				kk.updateGroup(G)
			except:
				try:
					G = kc.getGroup(grup)
					G.preventedJoinByTicket = True
					kc.updateGroup(G)
				except:
					try:
						G = kd.getGroup(grup)
						G.preventedJoinByTicket = True
						kd.updateGroup(G)
					except:
						try:
							G = ke.getGroup(grup)
							G.preventedJoinByTicket = True
							ke.updateGroup(G)
						except:
							try:
								G = a1.getGroup(grup)
								G.preventedJoinByTicket = True
								a1.updateGroup(G)
							except:
								try:
									G = a2.getGroup(grup)
									G.preventedJoinByTicket = True
									a2.updateGroup(G)
								except:
									try:
										G = a3.getGroup(grup)
										G.preventedJoinByTicket = True
										a3.updateGroup(G)
									except:
										pass

def kickprot(grup, target):
	try:
		asd= ki.kickoutFromGroup(grup, [target])
		if asd != None:
			sentinelfail
	except:
		try:
			asd= kk.kickoutFromGroup(grup, [target])
			if asd != None:
				sentinelfail
		except:
			try:
				asd= kc.kickoutFromGroup(grup, [target])
				if asd != None:
					sentinelfail
			except:
				try:
					asd= kd.kickoutFromGroup(grup, [target])
					if asd != None:
						sentinelfail
				except:
					try:
						asd= ke.kickoutFromGroup(grup, [target])
						if asd != None:
							sentinelfail
					except:
						try:
							asd= a1.kickoutFromGroup(grup, [target])
							if asd != None:
								sentinelfail
						except:
							try:
								asd= a2.kickoutFromGroup(grup, [target])
								if asd != None:
									sentinelfail
							except:
								try:
									asd= a3.kickoutFromGroup(grup, [target])
									if asd != None:
										sentinelfail
								except:
									pass

def cancelprot(grup, target):
	try:
		asd= ki.cancelGroupInvitation(grup, [target])
		if asd != None:
			sentinelfail
	except:
		try:
			asd= kk.cancelGroupInvitation(grup, [target])
			if asd != None:
				sentinelfail
		except:
			try:
				asd= kc.cancelGroupInvitation(grup, [target])
				if asd != None:
					sentinelfail
			except:
				try:
					asd= kd.cancelGroupInvitation(grup, [target])
					if asd != None:
						sentinelfail
				except:
					try:
						asd= ke.cancelGroupInvitation(grup, [target])
						if asd != None:
							sentinelfail
					except:
						try:
							asd= a1.cancelGroupInvitation(grup, [target])
							if asd != None:
								sentinelfail
						except:
							try:
								asd= a2.cancelGroupInvitation(grup, [target])
								if asd != None:
									sentinelfail
							except:
								try:
									asd= a2.cancelGroupInvitation(grup, [target])
									if asd != None:
										sentinelfail
								except:
									try:
										asd= cl.cancelGroupInvitation(grup, [target])
										if asd != None:
											sentinelfail
									except:
										pass

def inviteprot(grup, target):
	try:
		cl.findAndAddContactsByMid(target)
		asd= cl.inviteIntoGroup(grup, [target])
		if asd != None:
			sentinelfail
	except:
		try:
			ki.findAndAddContactsByMid(target)
			asd= ki.inviteIntoGroup(grup, [target])
			if asd != None:
				sentinelfail
		except:
			try:
				kk.findAndAddContactsByMid(target)
				asd= kk.inviteIntoGroup(grup, [target])
				if asd != None:
					sentinelfail
			except:
				try:
					kc.findAndAddContactsByMid(target)
					asd= kc.inviteIntoGroup(grup, [target])
					if asd != None:
						sentinelfail
				except:
					try:
						kd.findAndAddContactsByMid(target)
						asd= kd.inviteIntoGroup(grup, [target])
						if asd != None:
							sentinelfail
					except:
						try:
							ke.findAndAddContactsByMid(target)
							asd= ke.inviteIntoGroup(grup, [target])
							if asd != None:
								sentinelfail
						except:
							try:
								a1.findAndAddContactsByMid(target)
								asd= a1.inviteIntoGroup(grup, [target])
								if asd != None:
									sentinelfail
							except:
								try:
									a2.findAndAddContactsByMid(target)
									asd= a2.inviteIntoGroup(grup, [target])
									if asd != None:
										sentinelfail
								except:
									try:
										a3.findAndAddContactsByMid(target)
										asd= a3.inviteIntoGroup(grup, [target])
										if asd != None:
											sentinelfail
									except:
										pass

def backupprot(grup, target):
	try:
		cl.inviteIntoGroup(grup, [target])
		if target == mid:
			cl.acceptGroupInvitation(grup)
		if target == Amid:
			ki.acceptGroupInvitation(grup)
		if target == Bmid:
			kk.acceptGroupInvitation(grup)
		if target == Cmid:
			kc.acceptGroupInvitation(grup)
		if target == Dmid:
			kd.acceptGroupInvitation(grup)
		if target == Emid:
			ke.acceptGroupInvitation(grup)
		if target == Fmid:
			a1.acceptGroupInvitation(grup)
		if target == Gmid:
			a2.acceptGroupInvitation(grup)
		if target == Hmid:
			a3.acceptGroupInvitation(grup)
	except:
		try:
			ki.inviteIntoGroup(grup, [target])
			if target == mid:
				cl.acceptGroupInvitation(grup)
			if target == Amid:
				ki.acceptGroupInvitation(grup)
			if target == Bmid:
				kk.acceptGroupInvitation(grup)
			if target == Cmid:
				kc.acceptGroupInvitation(grup)
			if target == Dmid:
				kd.acceptGroupInvitation(grup)
			if target == Emid:
				ke.acceptGroupInvitation(grup)
			if target == Fmid:
				a1.acceptGroupInvitation(grup)
			if target == Gmid:
				a2.acceptGroupInvitation(grup)
			if target == Hmid:
				a3.acceptGroupInvitation(grup)
		except:
			try:
				kk.inviteIntoGroup(grup, [target])
				if target == mid:
					cl.acceptGroupInvitation(grup)
				if target == Amid:
					ki.acceptGroupInvitation(grup)
				if target == Bmid:
					kk.acceptGroupInvitation(grup)
				if target == Cmid:
					kc.acceptGroupInvitation(grup)
				if target == Dmid:
					kd.acceptGroupInvitation(grup)
				if target == Emid:
					ke.acceptGroupInvitation(grup)
				if target == Fmid:
					a1.acceptGroupInvitation(grup)
				if target == Gmid:
					a2.acceptGroupInvitation(grup)
				if target == Hmid:
					a3.acceptGroupInvitation(grup)
			except:
				try:
					kc.inviteIntoGroup(grup, [target])
					if target == mid:
						cl.acceptGroupInvitation(grup)
					if target == Amid:
						ki.acceptGroupInvitation(grup)
					if target == Bmid:
						kk.acceptGroupInvitation(grup)
					if target == Cmid:
						kc.acceptGroupInvitation(grup)
					if target == Dmid:
						kd.acceptGroupInvitation(grup)
					if target == Emid:
						ke.acceptGroupInvitation(grup)
					if target == Fmid:
						a1.acceptGroupInvitation(grup)
					if target == Gmid:
						a2.acceptGroupInvitation(grup)
					if target == Hmid:
						a3.acceptGroupInvitation(grup)
				except:
					try:
						kd.inviteIntoGroup(grup, [target])
						if target == mid:
							cl.acceptGroupInvitation(grup)
						if target == Amid:
							ki.acceptGroupInvitation(grup)
						if target == Bmid:
							kk.acceptGroupInvitation(grup)
						if target == Cmid:
							kc.acceptGroupInvitation(grup)
						if target == Dmid:
							kd.acceptGroupInvitation(grup)
						if target == Emid:
							ke.acceptGroupInvitation(grup)
						if target == Fmid:
							a1.acceptGroupInvitation(grup)
						if target == Gmid:
							a2.acceptGroupInvitation(grup)
						if target == Hmid:
							a3.acceptGroupInvitation(grup)
					except:
						try:
							ke.inviteIntoGroup(grup, [target])
							if target == mid:
								cl.acceptGroupInvitation(grup)
							if target == Amid:
								ki.acceptGroupInvitation(grup)
							if target == Bmid:
								kk.acceptGroupInvitation(grup)
							if target == Cmid:
								kc.acceptGroupInvitation(grup)
							if target == Dmid:
								kd.acceptGroupInvitation(grup)
							if target == Emid:
								ke.acceptGroupInvitation(grup)
							if target == Fmid:
								a1.acceptGroupInvitation(grup)
							if target == Gmid:
								a2.acceptGroupInvitation(grup)
							if target == Hmid:
								a3.acceptGroupInvitation(grup)
						except:
							try:
								a1.inviteIntoGroup(grup, [target])
								if target == mid:
									cl.acceptGroupInvitation(grup)
								if target == Amid:
									ki.acceptGroupInvitation(grup)
								if target == Bmid:
									kk.acceptGroupInvitation(grup)
								if target == Cmid:
									kc.acceptGroupInvitation(grup)
								if target == Dmid:
									kd.acceptGroupInvitation(grup)
								if target == Emid:
									ke.acceptGroupInvitation(grup)
								if target == Fmid:
									a1.acceptGroupInvitation(grup)
								if target == Gmid:
									a2.acceptGroupInvitation(grup)
								if target == Hmid:
									a3.acceptGroupInvitation(grup)
							except:
								try:
									a2.inviteIntoGroup(grup, [target])
									if target == mid:
										cl.acceptGroupInvitation(grup)
									if target == Amid:
										ki.acceptGroupInvitation(grup)
									if target == Bmid:
										kk.acceptGroupInvitation(grup)
									if target == Cmid:
										kc.acceptGroupInvitation(grup)
									if target == Dmid:
										kd.acceptGroupInvitation(grup)
									if target == Emid:
										ke.acceptGroupInvitation(grup)
									if target == Fmid:
										a1.acceptGroupInvitation(grup)
									if target == Gmid:
										a2.acceptGroupInvitation(grup)
									if target == Hmid:
										a3.acceptGroupInvitation(grup)
								except:
									try:
										a3.inviteIntoGroup(grup, [target])
										if target == mid:
											cl.acceptGroupInvitation(grup)
										if target == Amid:
											ki.acceptGroupInvitation(grup)
										if target == Bmid:
											kk.acceptGroupInvitation(grup)
										if target == Cmid:
											kc.acceptGroupInvitation(grup)
										if target == Dmid:
											kd.acceptGroupInvitation(grup)
										if target == Emid:
											ke.acceptGroupInvitation(grup)
										if target == Fmid:
											a1.acceptGroupInvitation(grup)
										if target == Gmid:
											a2.acceptGroupInvitation(grup)
										if target == Hmid:
											a3.acceptGroupInvitation(grup)
									except:
										pass

def waktu(secs):
    mins, secs = divmod(secs,60)
    hours, mins = divmod(mins,60)
    days, hours = divmod(hours,24)
    weeks, days = divmod(days,7)
    months, weeks = divmod(weeks,4)
    text = ""
    if months != 0: text += "%02d Months" % (months)
    if weeks != 0: text += " %02d Weeks" % (weeks)
    if days != 0: text += " %02d Days" % (days)
    if hours !=  0: text +=  " %02d Hours" % (hours)
    if mins != 0: text += " %02d Minutes" % (mins)
    if secs != 0: text += " %02d Seconds" % (secs)
    if text[0] == " ":
        text = text[1:]
    return text

def runtime(secs):
    mins, secs = divmod(secs,60)
    hours, mins = divmod(mins,60)
    days, hours = divmod(hours,24)
    weeks, days = divmod(days,7)
    months, weeks = divmod(weeks,4)
    text = ""
    if months != 0: text += "%02d Months" % (months)
    if weeks != 0: text += " %02d Weeks" % (weeks)
    if days != 0: text += " %02d Days" % (days)
    if hours !=  0: text +=  " %02d Hours" % (hours)
    if mins != 0: text += " %02d Minutes" % (mins)
    if secs != 0: text += " %02d Seconds" % (secs)
    if text[0] == " ":
        text = text[1:]
    return text

def mentionMembers(to, mids=[]):
    if myMid in mids: mids.remove(myMid)
    parsed_len = len(mids)//20+1
    result = '┏━━━「 Mention Members 」\n'
    mention = '@zeroxyuuki\n'
    no = 0
    for point in range(parsed_len):
        mentionees = []
        for mid in mids[point*20:(point+1)*20]:
            no += 1
            result += '┣ %i. %s' % (no, mention)
            slen = len(result) - 12
            elen = len(result) + 3
            mentionees.append({'S': str(slen), 'E': str(elen - 4), 'M': mid})
            if mid == mids[-1]:
                result += '┗━━━「 Mention Members 」\n'
        if result:
            if result.endswith('\n'): result = result[:-1]
            cl.sendMessage(to, result, {'MENTION': json.dumps({'MENTIONEES': mentionees})}, 0)
        result = ''
        
def mentions(to, text="", mids=[]):
    arrData = ""
    arr = []
    mention = "@Cerberus "
    if mids == []:
        raise Exception("Invalid mids")
    if "@!" in text:
        if text.count("@!") != len(mids):
            raise Exception("Invalid mids")
        texts = text.split("@!")
        textx = ""
        for mid in mids:
            textx += str(texts[mids.index(mid)])
            slen = len(textx)
            elen = len(textx) + 15
            arrData = {'S':str(slen), 'E':str(elen - 4), 'M':mid}
            arr.append(arrData)
            textx += mention
        textx += str(texts[len(mids)])
    else:
        textx = ""
        slen = len(textx)
        elen = len(textx) + 15
        arrData = {'S':str(slen), 'E':str(elen - 4), 'M':mids[0]}
        arr.append(arrData)
        textx += mention + str(text)
    cl.sendMessage(to, textx, {'AGENT_NAME':'LINE OFFICIAL', 'AGENT_LINK': 'line://ti/p/~{}'.format(cl.getProfile().userid), 'AGENT_ICON': "http://dl.profile.line-cdn.net/" + cl.getContact("ue19ebfbbbe4fb3703fc89448faa8c8f7").picturePath, 'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)
    
def logError(text):
    cl.log("[ ERROR ] {}".format(str(text)))
    tz = pytz.timezone("Asia/Jakarta")
    timeNow = datetime.now(tz=tz)
    timeHours = datetime.strftime(timeNow,"(%H:%M)")
    day = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday","Friday", "Saturday"]
    hari = ["Minggu", "Senin", "Selasa", "Rabu", "Kamis", "Jumat", "Sabtu"]
    bulan = ["Januari", "Februari", "Maret", "April", "Mei", "Juni", "Juli", "Agustus", "September", "Oktober", "November", "Desember"]
    inihari = datetime.now(tz=tz)
    hr = inihari.strftime('%A')
    bln = inihari.strftime('%m')
    for i in range(len(day)):
        if hr == day[i]: hasil = hari[i]
    for k in range(0, len(bulan)):
        if bln == str(k): bln = bulan[k-1]
    time = "{}, {} - {} - {} | {}".format(str(hasil), str(inihari.strftime('%d')), str(bln), str(inihari.strftime('%Y')), str(inihari.strftime('%H:%M:%S')))
    with open("logError.txt","a") as error:
        error.write("\n[ {} ] {}".format(str(time), text))

def siderMembers(to, mid):
    try:
        arrData = ""
        textx = "Allooo.. ".format(str(len(mid)))
        arr = []
        no = 1
        num = 2
        for i in mid:
            mention = "@x\n"
            slen = str(len(textx))
            elen = str(len(textx) + len(mention) - 1)
            arrData = {'S':slen, 'E':elen, 'M':i}
            arr.append(arrData)
            textx += mention+settings["mention"]
            if no < len(mid):
                no += 1
                textx += "%i. " % (num)
                num=(num+1)
            else:
                try:
                    no = "\n┗━━━「 {} 」".format(str(cl.getGroup(to).name))
                except:
                    no = "\n┗━━━「 Success 」"
        cl.sendMessage(to, textx, {'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)
    except Exception as error:
        cl.sendMessage(to, "[ INFO ] Error :\n" + str(error))

def welcomeMembers(to, mid):
    try:
        arrData = ""
        textx = "Hello  ".format(str(len(mid)))
        arr = []
        no = 1
        num = 2
        for i in mid:
            ginfo = cl.getGroup(to)
            mention = "@x\n"
            slen = str(len(textx))
            elen = str(len(textx) + len(mention) - 1)
            arrData = {'S':slen, 'E':elen, 'M':i}
            arr.append(arrData)
            textx += mention+settings["wmessage"]+"\nGroup Name : "+str(ginfo.name)
            if no < len(mid):
                no += 1
                textx += "%i " % (num)
                num=(num+1)
            else:
                try:
                    no = "\n┗━━━「 {} 」".format(str(cl.getGroup(to).name))
                except:
                    no = "\n┗━━━「 Success 」"
        cl.sendMessage(to, textx, {'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)
    except Exception as error:
        cl.sendMessage(to, "[ INFO ] Error :\n" + str(error))

def sendMention1(to, mid, firstmessage):
    try:
        arrData = ""
        text = "%s " %(str(firstmessage))
        arr = []
        mention = "@x \n"
        slen = str(len(text))
        elen = str(len(text) + len(mention) - 1)
        arrData = {'S':slen, 'E':elen, 'M':mid}
        arr.append(arrData)
        today = datetime.today()
        future = datetime(2018,3,1)
        hari = (str(future - today))
        comma = hari.find(",")
        hari = hari[:comma]
        teman = cl.getAllContactIds()
        gid = cl.getGroupIdsJoined()
        tz = pytz.timezone("Asia/Jakarta")
        timeNow = datetime.now(tz=tz)
        eltime = time.time() - mulai
        bot = runtime(eltime)
        text += mention+" Time : "+datetime.strftime(timeNow,'%H:%M:%S')+" GMT +7\n Group : "+str(len(gid))+"\n Friend : "+str(len(teman))+"\n Expired : In "+hari+"\n Date : "+datetime.strftime(timeNow,'%d/%m/%Y')+"\n Runtime : \n • "+bot
        cl.sendMessage(to, text, {'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)
    except Exception as error:
        cl.sendMessage(to, "[ INFO ] Error :\n" + str(error))
        
def sendMention(to, text="", mids=[]):
    arrData = ""
    arr = []
    mention = "@uwewxolin "
    if mids == []:
        raise Exception("Invalid mids")
    if "@!" in text:
        if text.count("@!") != len(mids):
            raise Exception("Invalid mids")
        texts = text.split("@!")
        textx = ""
        for mid in mids:
            textx += str(texts[mids.index(mid)])
            slen = len(textx)
            elen = len(textx) + 15
            arrData = {'S':str(slen), 'E':str(elen - 4), 'M':mid}
            arr.append(arrData)
            textx += mention
        textx += str(texts[len(mids)])
    else:
        textx = ""
        slen = len(textx)
        elen = len(textx) + 15
        arrData = {'S':str(slen), 'E':str(elen - 4), 'M':mids[0]}
        arr.append(arrData)
        textx += mention + str(text)
    cl.sendMessage(to, textx, {'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)
        
def sendMentionV2(to, text="", mids=[]):
    arrData = ""
    arr = []
    mention = "@zeroxyuuki "
    if mids == []:
        raise Exception("Invalid mids")
    if "@!" in text:
        if text.count("@!") != len(mids):
            raise Exception("Invalid mids")
        texts = text.split("@!")
        textx = ""
        for mid in mids:
            textx += str(texts[mids.index(mid)])
            slen = len(textx)
            elen = len(textx) + 15
            arrData = {'S':str(slen), 'E':str(elen - 4), 'M':mid}
            arr.append(arrData)
            textx += mention
        textx += str(texts[len(mids)])
    else:
        textx = ""
        slen = len(textx)
        elen = len(textx) + 15
        arrData = {'S':str(slen), 'E':str(elen - 4), 'M':mids[0]}
        arr.append(arrData)
        textx += mention + str(text)
    cl.sendMessage(to, textx, {'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)
    
def uwewwwMention(to, text="",ps='', mids=[]):
    arrData = ""
    arr = []
    mention = "@Cerberus "
    if mids == []:
        raise Exception("Invalid mids")
    if "@!" in text:
        if text.count("@!") != len(mids):
            raise Exception("Invalid mids")
        texts = text.split("@!")
        textx = ''
        h = ''
        for mid in range(len(mids)):
            h+= str(texts[mid].encode('unicode-escape'))
            textx += str(texts[mid])
            if h != textx:slen = len(textx)+h.count('U0');elen = len(textx)+h.count('U0') + 13
            else:slen = len(textx);elen = len(textx) + 13
            arrData = {'S':str(slen), 'E':str(elen), 'M':mids[mid]}
            arr.append(arrData)
            textx += mention
        textx += str(texts[len(mids)])
    else:
        textx = ''
        slen = len(textx)
        elen = len(textx) + 18
        arrData = {'S':str(slen), 'E':str(elen - 4), 'M':mids[0]}
        arr.append(arrData)
        textx += mention + str(text)
    try:
        cl.sendMessage(to, textx, {'MSG_SENDER_NAME': cl.getContact(ps).displayName,'MSG_SENDER_ICON': "https://os.line.naver.jp/os/p/"+ps,'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)
    except Exception as e:
        cl.sendMessage(to, textx, {'MSG_SENDER_NAME': cl.getContact(to).displayName,'MSG_SENDER_ICON': 'https://os.line.naver.jp/os/p/'+to,'MENTION': str('{"MENTIONEES":' + json.dumps(arr) + '}')}, 0)

def command(text):
    pesan = text.lower()
    if pesan.startswith(settings["keyCommand"]):
        cmd = pesan.replace(settings["keyCommand"],"")
    else:
        cmd = "command"
    return cmd

def removeCmd(cmd, text):
	key = settings["keyCommand"]
	if settings["setKey"] == False: key = ''
	rmv = len(key + cmd) + 1
	return text[rmv:]

def blacklist(target):
	if target in creator or target in owner or target in admin or target in staff or target in Bots or target in cerberusbots:
		pass
	else:
		status["blacklist"].append(target)

def backupData():
	try:
		backup = settings
		f = codecs.open('settings.json','w','utf-8')
		json.dump(backup, f, sort_keys=True, indent=4, ensure_ascii=False)
		return True
	except:
		pass

def debug():
	get_profile_time_start = time.time()
	get_profile = cl.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = ki.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = kk.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = kk.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = kc.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = kd.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = ke.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = a1.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = a2.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)
	get_profile_time_start = time.time()
	get_profile = a3.getProfile()
	get_profile_time = time.time() - get_profile_time_start
	get_profile_took = time.time() - get_profile_time_start
	return "「 Bots Speed 」\n • Took : %.3fms\n • Taken: %.5f" % (get_profile_took,get_profile_time)

def RECEIVE_MESSAGE(op):
	global cmd
	global text
	global groupParam
	msg = op.message
	text = msg.text
	reply = msg.id
	receiver = msg.to
	sender = msg._from
	if msg.toType == 0 or msg.toType == 1 or msg.toType == 2:
		if msg.toType == 0:
			if sender != cl.profile.mid:
				to = sender
			else:
				to = receiver
		if msg.toType == 1:
			to = receiver
		if msg.toType == 2:
			to = receiver
		if msg.contentType == 0:
			if text is None:
				return
			else:
				uwew = command(text)
				sentinel = " ".join(uwew.split())
			for sentinel in uwew.split(' & '):
				if sentinel == "tagall":
					members = []
					if msg.toType == 1:
						room = cl.getCompactRoom(receiver)
						members = [mem.mid for mem in room.contacts]
					elif msg.toType == 2:
						group = cl.getCompactGroup(receiver)
						members = [mem.mid for mem in group.members]
					else:
						return cl.sendReplyMessage(reply,receiver,"Use Only Group Chat")
					if members:
						mentionMembers(to, members)
				if sentinel == "cerberus:my grade":
					if sender in creator:
						sendMention(to,"\nYou're My Creator ^_^",[sender])
					if sender in owner:
						sendMention(to,"\nYou're My Owner ^_^",[sender])
					if sender in admin:
						sendMention(to,"\nYou're My Admin ^_^",[sender])
					if sender in staff:
						sendMention(to,"\nYou're My Staff ^_^",[sender])
					else:
						sendMention(to,"\nLu Siapa Anying?",[sender])
				if sentinel == "system" or sentinel == "about":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						rt = time.time() - programStart
						run = runtime(rt)
						cr = "ud5b11bf786ffbabd45a7a83157e3fbcc"
						make = cl.getContact(cr).displayName
						fakesp = '567'
						sp = "".join([random.choice(fakesp) for x in range(5)])
						hsl = "0.00" + sp
						fid = cl.getAllContactIds()
						frien = len(fid)
						bot = len(status["Bots"])
						own = len(status["owner"])
						adm = len(status["admin"])
						stf = len(status["staff"])
						ac = subprocess.getoutput('lsb_release -a')
						am = subprocess.getoutput('cat /proc/meminfo')
						ax = subprocess.getoutput('lscpu')
						core = subprocess.getoutput('grep -c ^processor /proc/cpuinfo ')
						python_imp = platform.python_implementation()
						python_ver = platform.python_version()
						for line in ac.splitlines():
							if 'Description:' in line:
								os = line.split('Description:')[1].replace(' ','')
						for line in ax.splitlines():
							if 'Architecture:' in line:
								architecture =  line.split('Architecture:')[1].replace(' ','')
						for line in am.splitlines():
							if 'MemTotal:' in line:
								mem = line.split('MemTotal:')[1].replace(' ','')
							if 'MemFree:' in line:
								fr = line.split('MemFree:')[1].replace(' ','')
						res = "┏━━━「 About Bots 」"
						res += "\n┣ Creator : {}".format(make)
						res += "\n┣ Owner : {}".format(own)
						res += "\n┣ Admin : {}".format(adm)
						res += "\n┣ Staff : {}".format(stf)
						res += "\n┣ Bots : {}".format(bot)
						res += "\n┣ Friends : {}".format(frien)
						res += "\n┣ Runtime : {}".format(run)
						res += "\n┣ Response : {} secs".format(hsl)
						res += "\n┣━「 About System 」"
						res += "\n┣ CPU Core : {}".format(core)
						res += "\n┣ Total Memory: {}".format(mem)
						res += "\n┣ Free Memory: {}".format(fr)
						res += "\n┣ Architecture: {}".format(architecture)
						res += "\n┣ OS: {}".format(os)
						res += "\n┣ Language: {}".format(python_imp)
						res += "\n┣ Version: {}".format(python_ver)
						res += "\n┗━━━"
						cl.sendReplyMessage(reply,receiver,res)
				if sentinel == "cerberus:commands":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						res = "┏━━━━━━━━"
						res += "\n┣ Bots Name : %s" % cl.profile.displayName
						res += "\n┣ Prefix : 「 {} 」 ".format(str(settings["keyCommand"]))
						res += "\n┣━━━━━━━━"
						res += "\n┣ Cerberus:Commands"
						res += "\n┣ Cerberus:Setbot"
						res += "\n┣ Cerberus:Speed"
						res += "\n┣ Cerberus:Inviteall"
						res += "\n┣ Cerberus:Qrjoin"
						res += "\n┣ Cerberus:Byeall"
						res += "\n┣ Cerberus:Rname"
						res += "\n┣ Cerberus:Grouplist"
						res += "\n┣ Cerberus:Clearchat"
						res += "\n┣ Cerberus:Opcancel"
						res += "\n┣ Cerberus:Purge"
						res += "\n┣ Cerberus:Checkbot"
						res += "\n┣ Cerberus:Reboot System"
						res += "\n┣ Cerberus:Clearban"
						res += "\n┣ Cerberus:Blacklist User"
						res += "\n┣ Cerberus:View Grade"
						res += "\n┣ Cerberus:View Bots"
						res += "\n┣ Cerberus:Kick「 Mention 」"
						res += "\n┣ Cerberus:Owner:add「 Mention 」"
						res += "\n┣ Cerberus:Owner:dell「 Mention 」"
						res += "\n┣ Cerberus:Admin:add「 Mention 」"
						res += "\n┣ Cerberus:Admin:dell「 Mention 」"
						res += "\n┣ Cerberus:Staff:add「 Mention 」"
						res += "\n┣ Cerberus:Staff:dell「 Mention 」"
						res += "\n┣ Cerberus:Bots:add「 Mention 」"
						res += "\n┣ Cerberus:Bots:dell「 Mention 」"
						res += "\n┣ Cerberus:Ban「 Mention 」"
						res += "\n┣ Cerberus:Unban「 Mention 」"
						res += "\n┣ Cerberus:Changename:All/1-9/Ghost「 Name 」"
						res += "\n┣ Cerberus:Changebio:All/1-9/Ghost「 Name 」"
						res += "\n┣ Cerberus:Changepict:All/1-9/Ghost"
						res += "\n┣ Cerberus:OwnerAdd: 「 On/Off 」"
						res += "\n┣ Cerberus:OwnerDell: 「 On/Off 」"
						res += "\n┣ Cerberus:AdminAdd: 「 On/Off 」"
						res += "\n┣ Cerberus:AdminDell: 「 On/Off 」"
						res += "\n┣ Cerberus:StaffAdd: 「 On/Off 」"
						res += "\n┣ Cerberus:StaffDell: 「 On/Off 」"
						res += "\n┣ Cerberus:BotsAdd: 「 On/Off 」"
						res += "\n┣ Cerberus:BotsDell: 「 On/Off 」"
						res += "\n┣ Cerberus:BanAdd: 「 On/Off 」"
						res += "\n┣ Cerberus:BanDell: 「 On/Off 」"
						res += "\n┗━━━━━━━━"
						cl.sendReplyMessage(reply,receiver,res)
				if sentinel == "cerberus:purge":
					if sender in creator or sender in owner:
						group = cl.getGroup(receiver)
						gMembMids = [contact.mid for contact in group.members]
						match = []
						for target in ban["blacklist"]:
							match+=filter(lambda str: str == target, gMembMids)
						if match == []:
							cl.sendReplyMessage(reply,receiver,"Nothing -_-")
							return
						for itunya in match:
							try:
								kickk = threading.Thread(target=kickprot, args=(receiver, itunya)).start()
							except:
								pass
				if sentinel == "cerberus:opcancel":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						settings["addowner"] = False
						settings["addowner"] = False
						settings["addadmin"] = False
						settings["delladmin"] = False
						settings["addstaff"] = False
						settings["dellstaff"] = False
						settings["addbots"] = False
						settings["dellbots"] = False
						settings["addban"] = False
						settings["dellban"] = False
						cl.sendReplyMessage(reply,receiver,"「 All Operation Aborted 」")
				if sentinel == "cerberus:clearchat":
					if sender in creator or sender in owner:
						a = [cl,ki,kk,kc,kd,ke,a1,a2,a3,sw]
						b = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
						for u in a:
							u.removeAllMessages(op.param2)
						for h in b:
							h.sendReplyMessage(reply,receiver,"「 All Chat Cleared 」")
				if sentinel == "cerberus:speed":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						cl.sendReplyMessage(reply,receiver,debug())
						ki.sendReplyMessage(reply,receiver,debug())
						kk.sendReplyMessage(reply,receiver,debug())
						kc.sendReplyMessage(reply,receiver,debug())
						kd.sendReplyMessage(reply,receiver,debug())
						ke.sendReplyMessage(reply,receiver,debug())
						a1.sendReplyMessage(reply,receiver,debug())
						a2.sendReplyMessage(reply,receiver,debug())
						a3.sendReplyMessage(reply,receiver,debug())
				if sentinel == "cerberus:rname":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						cl.sendReplyMessage(reply,receiver,sname1)
						ki.sendReplyMessage(reply,receiver,sname2)
						kk.sendReplyMessage(reply,receiver,sname3)
						kc.sendReplyMessage(reply,receiver,sname4)
						kd.sendReplyMessage(reply,receiver,sname5)
						ke.sendReplyMessage(reply,receiver,sname6)
						a1.sendReplyMessage(reply,receiver,sname7)
						a2.sendReplyMessage(reply,receiver,sname8)
						a3.sendReplyMessage(reply,receiver,sname9)
				if sentinel == "cerberus:inviteall":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						try:
							bot = [Amid,Bmid,Cmid,Dmid,Emid,Fmid,Gmid,Hmid]
							cl.inviteIntoGroup(receiver,bot)
							ki.acceptGroupInvitation(receiver)
							kk.acceptGroupInvitation(receiver)
							kc.acceptGroupInvitation(receiver)
							kd.acceptGroupInvitation(receiver)
							ke.acceptGroupInvitation(receiver)
							a1.acceptGroupInvitation(receiver)
							a2.acceptGroupInvitation(receiver)
							a3.acceptGroupInvitation(receiver)
						except:
							cl.sendReplyMessage(reply,receiver,"「 Limit -_- 」")
				if sentinel == "cerberus:ghostjoin":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						G = cl.getGroup(receiver)
						G.preventedJoinByTicket = False
						cl.updateGroup(G)
						group = cl.reissueGroupTicket(receiver)
						sw.acceptGroupInvitationByTicket(receiver, group)
						G.preventedJoinByTicket = True
						cl.updateGroup(G)
				if sentinel == "cerberus:qrjoin":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						G = cl.getGroup(receiver)
						G.preventedJoinByTicket = False
						cl.updateGroup(G)
						Ridwan = cl.reissueGroupTicket(receiver)
						for anu in Team:
							try:
								anu.acceptGroupInvitationByTicket(receiver,Ridwan)
							except:
								pass
						G.preventedJoinByTicket = True
						cl.updateGroup(G)
				if sentinel.startswith("respon:"):
					if sender in creator or sender in owner:
						sep = text.split(":")
						say = text.replace(sep[0] + ":","")
						cc = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
						for aa in cc:
							aa.sendReplyMessage(reply,receiver,say)
				if sentinel.startswith("openqr:"):
					if sender in creator or sender in owner:
						sep = text.split(":")
						number = text.replace(sep[0] + ":","")
						groups = cl.getGroupIdsJoined()
						group = groups[int(number)-1]
						G = cl.getGroup(group)
						G.preventedJoinByTicket = False
						cl.updateGroup(G)
						url = cl.reissueGroupTicket(group)
						ticket = 'https://line.me/R/ti/g/{}'.format(url)
						cl.sendReplyMessage(reply,receiver,ticket)
				if sentinel.startswith("group:invite "):
					if sender in creator or sender in owner:
						separate = text.split(" ")
						num = text.replace(separate[0] + " ","")
						groups = cl.getGroupIdsJoined()
						if groups is not None:
							if int(num) <= len(groups):
								groupid = groups[int(num) - 1]
								group = cl.getGroup(groupid)
								try:
									anjanj = threading.Thread(target=inviteprot, args=(groupid, sender)).start()
									cl.sendReplyMessage(reply,receiver, "「 Done invite to " + group.name + " 」")
								except Exception as e:
									cl.sendReplyMessage(reply,receiver,"「 Limit -_- 」")
				if sentinel.startswith("cerberus:group:joinall "):
					if sender in creator or sender in owner:
						separate = text.split(" ")
						number = text.replace(separate[0] + " ","")
						groups = cl.getGroupIdsJoined()
						gname = cl.getGroup(receiver).name
						try:
							group = groups[int(number)-1]
							name = cl.getContact(sender).displayName
							cl.sendMessage(group,"「 Remote Command 」\nAll Bots Will Joined On This Group\n Command By {}\nFrom Group:{}".format(name,gname))
							G = cl.getGroup(group)
							G.preventedJoinByTicket = False
							cl.updateGroup(G)
							Wew = cl.reissueGroupTicket(group)
							aa = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
							for uu in aa:
								uu.acceptGroupInvitationByTicket(group,Wew)
							G = cl.getGroup(group)
							G.preventedJoinByTicket = True
							cl.updateGroup(G)
							cl.sendReplyMessage(reply,receiver,"Success Sent Remote Command To Group : {}".format(cl.getGroup(group).name))
						except Exception as error:
							cl.sendReplyMessage(reply,receiver,error)
				if sentinel.startswith("cerberus:grouplist"):
					if sender in creator or sender in owner:
						ma = ""
						a = 0
						gid = cl.getGroupIdsJoined()
						for i in gid:
							G = cl.getGroup(i)
							a = a + 1
							end = "\n"
							ma += "┣ " + str(a) + ". " +G.name+ "\n"
						cl.sendReplyMessage(msg.id, to, "┏━━━\n┣━━「 Group List 」\n"+ma+"┗━━ 「 Total : "+str(len(gid))+" Groups 」")
				if sentinel.startswith("cerberus:owner:add"):
					if sender in creator:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						bot = [cl,ki,kk,kc,kd,ke,a1,a2,a3,sw]
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for itu in bot:
							for haha in targets:
								try:
									itu.findAndAddContactsByMid(haha)
								except:
									pass
						for target in targets:
							try:
								status["owner"].append(target)
								sendMention(to,"「 Grant Access 」\nUser @! Promoted To Owner Access ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nCreator Permission -_-")
				if sentinel.startswith("cerberus:owner:dell"):
					if sender in creator:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for target in targets:
							try:
								status["owner"].remove(target)
								sendMention(to,"「 Grant Access 」\nUser @! Deleted From Owner Access ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nCreator Permission -_-")
				if sentinel.startswith("cerberus:admin:add"):
					if sender in creator or sender in owner:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						bot = [cl,ki,kk,kc,kd,ke,a1,a2,a3,sw]
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for itu in bot:
							for haha in targets:
								try:
									itu.findAndAddContactsByMid(haha)
								except:
									pass
						for target in targets:
							try:
								status["admin"].append(target)
								sendMention(to,"「 Grant Access 」\nUser @! Promoted To Admin Access ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nOwner Permission -_-")
				if sentinel.startswith("cerberus:admin:dell"):
					if sender in creator or sender in owner:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for target in targets:
							try:
								status["admin"].remove(target)
								sendMention(to,"「 Grant Access 」\nUser @! Deleted From Admin Access ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nOwner Permission -_-")
				if sentinel.startswith("cerberus:staff:add"):
					if sender in creator or sender in owner or sender in admin:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						bot = [cl,ki,kk,kc,kd,ke,a1,a2,a3,sw]
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for itu in bot:
							for haha in targets:
								try:
									itu.findAndAddContactsByMid(haha)
								except:
									pass
						for target in targets:
							try:
								status["staff"].append(target)
								sendMention(to,"「 Grant Access 」\nUser @! Promoted To Staff Access ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nOwner/Admin Permission -_-")
				if sentinel.startswith("cerberus:staff:dell"):
					if sender in creator or sender in owner or sender in admin:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for target in targets:
							try:
								status["staff"].remove(target)
								sendMention(to,"「 Grant Access 」\nUser @! Deleted From Staff Access ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nOwner/Admin Permission -_-")
				if sentinel.startswith("cerberus:bots:add"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						bot = [cl,ki,kk,kc,kd,ke,a1,a2,a3,sw]
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for itu in bot:
							for haha in targets:
								try:
									itu.findAndAddContactsByMid(haha)
								except:
									pass
						for target in targets:
							try:
								status["Bots"].append(target)
								sendMention(to,"「 Bots List 」\nUser @! Promoted To Bots ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Owner/Admin/Staff Permission -_- 」")
				if sentinel.startswith("cerberus:bots:dell"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for target in targets:
							try:
								status["Bots"].remove(target)
								sendMention(to,"「 Bots List 」\nUser @! Deleted From Bots ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Owner/Admin/Staff Permission -_- 」")
				if sentinel.startswith("cerberus:ban"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for target in targets:
							if target in creator:
								sendMention(to,"「 Blacklist 」\n@! Is Your Creator Idiot -_-",[target])
								pass
							if target in owner:
								sendMention(to,"「 Blacklist 」\n@! Is Your Owner Idiot -_-",[target])
								pass
							else:
								try:
									ban["blacklist"].append(target)
									sendMention(to,"「 Blacklist 」\nUser @! Added To Blacklist User ^_^",[target])
								except:
									pass
				if sentinel.startswith("cerberus:unban"):
					if sender in creator or sender in owner:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for target in targets:
							try:
								ban["blacklist"].remove(target)
								sendMention(to,"「 Blacklist 」\nUser @! Deleted From Blacklist User ^_^",[target])
							except:
								pass
					else:
						cl.sendReplyMessage(reply,receiver,"「 Owner Permission -_- 」")
				if sentinel.startswith("cerberus:auto purge "):
					if sender in creator or sender in owner:
						spl = sentinel.replace("cerberus:auto purge ","")
						if spl == "on":
							settings["autoPurge"] = True
							cl.sendReplyMessage(reply,receiver,"「 Purge Blacklist Set To On 」")
						if spl == "off":
							settings["autoPurge"] = False
							cl.sendReplyMessage(reply,receiver,"「 Purge Blacklist Set To Off 」")
				if sentinel.startswith("cerberus:owneradd:"):
					if sender in creator:
						spl = sentinel.replace("cerberus:owneradd:","")
						if spl == "on":
							settings["addowner"] = True
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nPlease Send Contact To Add ^_^")
						if spl == "off":
							settings["addowner"] = False
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nAdd Owner Canceled ^_^")
				if sentinel.startswith("cerberus:ownerdell:"):
					if sender in creator:
						spl = sentinel.replace("cerberus:ownerdell:","")
						if spl == "on":
							settings["dellowner"] = True
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nPlease Send Contact To Delete ^_^")
						if spl == "off":
							settings["dellowner"] = False
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nDelete Owner Canceled ^_^")
				if sentinel.startswith("cerberus:adminadd:"):
					if sender in creator or sender in owner:
						spl = sentinel.replace("cerberus:adminadd:","")
						if spl == "on":
							settings["addadmin"] = True
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nPlease Send Contact To Add ^_^")
						if spl == "off":
							settings["addadmin"] = False
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nAdd Admin Canceled ^_^")
				if sentinel.startswith("cerberus:admindell:"):
					if sender in creator or sender in owner:
						spl = sentinel.replace("cerberus:admindell:","")
						if spl == "on":
							settings["delladmin"] = True
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nPlease Send Contact To Delete ^_^")
						if spl == "off":
							settings["delladmin"] = False
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nDelete Admin Canceled ^_^")
				if sentinel.startswith("cerberus:staffadd:"):
					if sender in creator or sender in owner or sender in admin:
						spl = sentinel.replace("cerberus:staffadd:","")
						if spl == "on":
							settings["addadmin"] = True
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nPlease Send Contact To Add ^_^")
						if spl == "off":
							settings["addadmin"] = False
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nAdd Staff Canceled ^_^")
				if sentinel.startswith("cerberus:staffdell:"):
					if sender in creator or sender in owner or sender in admin:
						spl = sentinel.replace("cerberus:staffdell:","")
						if spl == "on":
							settings["dellstaff"] = True
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nPlease Send Contact To Delete ^_^")
						if spl == "off":
							settings["dellstaff"] = False
							cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nDelete Staff Canceled ^_^")
				if sentinel.startswith("cerberus:botsadd:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:botsadd:","")
						if spl == "on":
							settings["addbots"] = True
							cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nPlease Send Contact To Add ^_^")
						if spl == "off":
							settings["addbots"] = False
							cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nAdd Bots Canceled ^_^")
				if sentinel.startswith("cerberus:botsdell:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:botsdell:","")
						if spl == "on":
							settings["dellbots"] = True
							cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nPlease Send Contact To Delete ^_^")
						if spl == "off":
							settings["dellbots"] = False
							cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nDelete Bots Canceled ^_^")
				if sentinel.startswith("cerberus:banadd:"):
					if sender in creator or sender in owner:
						spl = sentinel.replace("cerberus:banadd:","")
						if spl == "on":
							settings["addban"] = True
							cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nPlease Send Contact To Add ^_^")
						if spl == "off":
							settings["addban"] = False
							cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nAdd User Blacklist Canceled ^_^")
				if sentinel.startswith("cerberus:bandell:"):
					if sender in creator or sender in owner:
						spl = sentinel.replace("cerberus:bandell:","")
						if spl == "on":
							settings["dellban"] = True
							cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nPlease Send Contact To Delete ^_^")
						if spl == "off":
							settings["dellban"] = False
							cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nDelete User Blacklist Canceled ^_^")
				if sentinel.startswith("cerberuse:war mode:"):
					if sender in creator or sender in owner:
						spl = sentinel.replace("cerberus:war mode:","")
						if spl == "on":
							if receiver in settings["warmode"]:
								uwew = "War Mode Already Active -_-"
							else:
								settings["warmode"].append(receiver)
								uwew = "War Mode Activated\nPlease Use This Mode Carefully"
							cl.sendReplyMessage(reply,receiver,"「 WARNING! 」\n" + uwew)
						if spl == "off":
							if receiver in settings["warmode"]:
								settings["warmode"].remove(receiver)
								uwew = "War Mode Deactivated\nNow Bots Back To Normal Mode"
							else:
								uwew = "War Mode Already Deactive -_-"
							cl.sendReplyMessage(reply,receiver,"「 WARNING! 」\n" + uwew)
				if sentinel.startswith("cerberus:max protection:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:max protection:","")
						if spl == "on":
							if receiver in settings["lockname"]:
								uwew = ""
							else:
								settings["lockname"].append(receiver)
								settings["lock_name"][receiver] = cl.getGroup(receiver).name
							if receiver in settings["antijs"]:
								uwew = ""
							else:
								sntnel16 = threading.Thread(target=inviteprot, args=(receiver, Zmid)).start()
								settings["antijs"].append(receiver)
							if receiver in settings["lockqr"]:
								uwew = ""
							else:
								settings["lockqr"].append(receiver)
							if receiver in settings["protect"]:
								uwew = ""
							else:
								settings["protect"].append(receiver)
							if receiver in settings["denyinvite"]:
								uwew = "Maximum Protection Already Enabled"
							else:
								settings["denyinvite"].append(receiver)
								info = cl.getGroup(receiver)
								uwew = "Maximum Protection Has Been Enabled\nOn Group: " +str(info.name)
							cl.sendReplyMessage(reply,receiver,"「 All Protection 」\n" + uwew)
						if spl == "off":
							if receiver in settings["lockname"]:
								settings["lockname"].remove(receiver)
								del settings["lock_name"][receiver]
								uwew = ""
							else:
								uwew = ""
							if receiver in settings["denyinvite"]:
								settings["denyinvite"].remove(receiver)
								uwew = ""
							else:
								uwew = ""
							if receiver in settings["lockqr"]:
								settings["lockqr"].remove(receiver)
								uwew = ""
							else:
								uwew = ""
							if receiver in settings["antijs"]:
								settings["antijs"].remove(receiver)
								info = cl.getGroup(receiver)
								uwew = "Maximum Protection Disabled\nOn Group: " +str(info.name)
							else:
								uwew = "Maximum Protection Already Disabled -_-"
							cl.sendReplyMessage(reply,receiver,"「 Maximum Protection 」\n" + uwew)
				if sentinel.startswith("cerberus:lock name:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:lock name:","")
						if spl == "on":
							if receiver in settings["lockname"]:
								uwew = "Group Lock Name Already Enabled -_-"
							else:
								settings["lockname"].append(receiver)
								settings["lock_name"][receiver] = cl.getGroup(receiver).name
								info = cl.getGroup(receiver)
								uwew = "Group Lock Name Enabled\nOn Group: " +str(info.name)
							cl.sendReplyMessage(reply,receiver,"「 Group Lock Name 」\n" + uwew)
						if spl == "off":
							if receiver in settings["lockname"]:
								settings["lockname"].remove(receiver)
								del settings["lock_name"][receiver]
								info = cl.getGroup(receiver)
								uwew = "Group Lock Name Disabled\nOn Group: " +str(info.name)
							else:
								uwew = "Group Lock Name Already Disabled -_-"
							cl.sendReplyMessage(reply,receiver,"「 Group Lock Name 」\n" + uwew)
				if sentinel.startswith("cerberus:deny invite:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:deny invite:","")
						if spl == "on":
							if receiver in settings["denyinvite"]:
								uwew = "Deny Invitation Already Enabled -_-"
							else:
								settings["denyinvite"].append(receiver)
								info = cl.getGroup(receiver)
								uwew = "Deny Invitation Enabled\nOn Group: " +str(info.name)
							cl.sendReplyMessage(reply,receiver,"「 Deny Invitation 」\n" + uwew)
						if spl == "off":
							if receiver in settings["denyinvite"]:
								settings["denyinvite"].remove(receiver)
								info = cl.getGroup(receiver)
								uwew = "Deny Invitation Disabled\nOn Group: " +str(info.name)
							else:
								uwew = "Deny Invitation Already Disabled -_-"
							cl.sendReplyMessage(reply,receiver,"「 Deny Invitation 」\n" + uwew)
				if sentinel.startswith("cerberus:group protection:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:group protection:","")
						if spl == "on":
							if receiver in settings["protect"]:
								uwew = "Group Protection Already Enabled -_-"
							else:
								settings["protect"].append(receiver)
								info = cl.getGroup(receiver)
								uwew = "Group Protection Enabled\nOn Group: " +str(info.name)
							cl.sendReplyMessage(reply,receiver,"「 Group Protection 」\n" + uwew)
						if spl == "off":
							if receiver in settings["protect"]:
								settings["protect"].remove(receiver)
								info = cl.getGroup(receiver)
								uwew = "Group Protection Disabled\nOn Group: " +str(info.name)
							else:
								uwew = "Group Protection Already Disabled -_-"
							cl.sendReplyMessage(reply,receiver,"「 Group Protection 」\n" + uwew)
				if sentinel.startswith("cerberus:lock qr:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:lock qr:","")
						if spl == "on":
							if receiver in settings["lockqr"]:
								uwew = "QR Lock Already Enabled -_-"
							else:
								settings["lockqr"].append(receiver)
								info = cl.getGroup(receiver)
								uwew = "QR Lock Enabled\nOn Group: " +str(info.name)
							cl.sendReplyMessage(reply,receiver,"「 QR Protection 」\n" + uwew)
						if spl == "off":
							if receiver in settings["lockqr"]:
								settings["lockqr"].remove(receiver)
								info = cl.getGroup(receiver)
								uwew = "QR Lock Disabled\nOn Group: " +str(info.name)
							else:
								uwew = "QR Lock Already Disabled -_-"
							cl.sendReplyMessage(reply,receiver,"「 QR Protection 」\n" + uwew)
				if sentinel.startswith("cerberus:js protection:"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						spl = sentinel.replace("cerberus:js protection:","")
						if spl == "on":
							if receiver in settings["antijs"]:
								uwew = "JS Protection Already Enabled -_-"
							else:
								sntnel15 = threading.Thread(target=inviteprot, args=(receiver, Zmid)).start()
								settings["antijs"].append(receiver)
								info = cl.getGroup(receiver)
								uwew = "JS Protection Enabled\nOn Group: " +str(info.name)
							cl.sendReplyMessage(reply,receiver,"「 JS Protection 」\n" + uwew)
						if spl == "off":
							if receiver in settings["antijs"]:
								settings["antijs"].remove(receiver)
								info = cl.getGroup(receiver)
								uwew = "JS Protection Disabled\nOn Group: " +str(info.name)
							else:
								uwew = "JS Protection Already Disabled -_-"
							cl.sendReplyMessage(reply,receiver,"「 JS Protection 」\n" + uwew)
				if sentinel.startswith("cerberus:setbot"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						md = "┏━━━「 Bots Settings 」\n"
						if settings["autoPurge"] == True: md+="┣ Auto Purge 「🔒」\n"
						else: md+="┣ Auto Purge 「🔓」\n"
						if settings["addowner"] == True: md+="┣ Add Owner 「🔒」\n"
						else: md+="┣ Add Owner 「🔓」\n"
						if settings["dellowner"] == True: md+="┣ Delete Owner 「🔒」\n"
						else: md+="┣ Delete Owner 「🔓」\n"
						if settings["addadmin"] == True: md+="┣ Add Admin 「🔒」\n"
						else: md+="┣ Add Admin 「🔓」\n"
						if settings["delladmin"] == True: md+="┣ Delete Admin 「🔒」\n"
						else: md+="┣ Delete Admin 「🔓」\n"
						if settings["addstaff"] == True: md+="┣ Add Staff 「🔒」\n"
						else: md+="┣ Add Staff 「🔓」\n"
						if settings["dellstaff"] == True: md+="┣ Delete Staff 「🔒」\n"
						else: md+="┣ Delete Staff 「🔓」\n"
						if settings["addbots"] == True: md+="┣ Add Bots 「🔒」\n"
						else: md+="┣ Add Bots 「🔓」\n"
						if settings["dellbots"] == True: md+="┣ Delete Bots 「🔒」\n"
						else: md+="┣ Delete Bots 「🔓」\n"
						if settings["addban"] == True: md+="┣ Add Blacklist 「🔒」\n"
						else: md+="┣ Add Blacklist 「🔓」\n"
						if settings["dellban"] == True: md+="┣ Delete Blacklist 「🔒」\n"
						else: md+="┣ Delete Blacklist 「🔓」\n"
						if receiver in settings["lockqr"]: md+="┣ QR Lock 「🔒」\n"
						else: md+="┣ QR Lock 「🔓」\n"
						if receiver in settings["protect"]: md+="┣ Group Protection 「🔒」\n"
						else: md+="┣ Group Protection 「🔓」\n"
						if receiver in settings["denyinvite"]: md+="┣ Deny Invitation 「🔒」\n"
						else: md+="┣ Deny Invitation 「🔓」\n"
						if receiver in settings["lockname"]: md+="┣ Group Lock Name 「🔒」\n"
						else: md+="┣ Group Lock Name 「🔓」\n"
						if receiver in settings["antijs"]: md+="┣ JS Protection 「🔒」\n"
						else: md+="┣ JS Protection 「🔓」\n"
						if receiver in settings["warmode"]: md+="┣ War Mode「🔒」"
						else: md+="┣ War Mode 「🔓」"
						ret_ = str(md)
						ret_ += "\n┣━━「 Protect Command 」"
						ret_ += "\n┣ Cerberus:Js Protection:「 On/Off 」"
						ret_ += "\n┣ Cerberus:Lock Qr:「 On/Off 」"
						ret_ += "\n┣ Cerberus:Deny Invite:「 On/Off 」"
						ret_ += "\n┣ Cerberus:Group Protection:「 On/Off 」"
						ret_ += "\n┣ Cerberus:Lock Name:「 On/Off 」"
						ret_ += "\n┣ Cerberus:Max Protection:「 On/Off 」"
						ret_ += "\n┣ Cerberus:War Mode:「 On/Off 」"
						ret_ += "\n┣━━「 Symbol Details 」"
						ret_ += "\n┣「🔒」: On/True/Enabled"
						ret_ += "\n┣「🔓」: Off/False/Disabled"
						ret_ += "\n┗━━━"
						cl.sendReplyMessage(reply,receiver,ret_)
				if sentinel.startswith("cerberus:checkbot"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						try:cl.inviteIntoGroup(to, ["u3529bce86ebac075d621966ef16486f3"]);has = "OK"
						except:has = "NOT"
						try:cl.kickoutFromGroup(to, ["u3529bce86ebac075d621966ef16486f3"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						cl.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:ki.inviteIntoGroup(to, ["u7d4e23945e41b5274455b95ffd8af1f1"]);has = "OK"
						except:has = "NOT"
						try:ki.kickoutFromGroup(to, ["u7d4e23945e41b5274455b95ffd8af1f1"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						ki.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:kk.inviteIntoGroup(to, ["u6c88002aed5c104ad6c4c878d89d7d07"]);has = "OK"
						except:has = "NOT"
						try:kk.kickoutFromGroup(to, ["u6c88002aed5c104ad6c4c878d89d7d07"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						kk.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:kc.inviteIntoGroup(to, ["u1b227c131d7829e69956c06ff6db572c"]);has = "OK"
						except:has = "NOT"
						try:kc.kickoutFromGroup(to, ["u1b227c131d7829e69956c06ff6db572c"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						kc.sendReplyMessage(msg.id, to, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:kd.inviteIntoGroup(to, ["udc7333bc03689e1eb494e4db5907e4f3"]);has = "OK"
						except:has = "NOT"
						try:kd.kickoutFromGroup(to, ["udc7333bc03689e1eb494e4db5907e4f3"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						kd.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:ke.inviteIntoGroup(to, ["u2d0a791fd3294afac34446593332a74b"]);has = "OK"
						except:has = "NOT"
						try:ke.kickoutFromGroup(to, ["u2d0a791fd3294afac34446593332a74b"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						ke.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:a1.inviteIntoGroup(to, ["u734f29aae0e572a358d9e499ade73639"]);has = "OK"
						except:has = "NOT"
						try:a1.kickoutFromGroup(to, ["u734f29aae0e572a358d9e499ade73639"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						a1.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:a2.inviteIntoGroup(to, ["u8bb5a06bb4420b91b1b7d7a47450e26b"]);has = "OK"
						except:has = "NOT"
						try:a2.kickoutFromGroup(to, ["u8bb5a06bb4420b91b1b7d7a47450e26b"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						a2.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
						try:a3.inviteIntoGroup(to, ["u1eedd8a03bee09b3bd7df0a3b4bab51c"]);has = "OK"
						except:has = "NOT"
						try:a3.kickoutFromGroup(to, ["u1eedd8a03bee09b3bd7df0a3b4bab51c"]);has1 = "OK"
						except:has1 = "NOT"
						if has == "OK":sil = "Normal~"
						else:sil = "Down!"
						if has1 == "OK":sil1 = "Normal~"
						else:sil1 = "Down!"
						a3.sendReplyMessage(reply, receiver, "「 Bots Status 」\n • Invite : {}\n • Kick : {}".format(sil1,sil))
				if sentinel.startswith("cerberus:limit @bye"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						try:cl.kickoutFromGroup(to, ["u3529bce86ebac075d621966ef16486f3"]);has = "OK"
						except:has = "NOT"
						if has == "OK":cl.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:cl.leaveGroup(receiver)
						try:ki.kickoutFromGroup(to, ["u7d4e23945e41b5274455b95ffd8af1f1"]);has = "OK"
						except:has = "NOT"
						if has == "OK":ki.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:ki.leaveGroup(receiver)
						try:kk.kickoutFromGroup(to, ["u6c88002aed5c104ad6c4c878d89d7d07"]);has = "OK"
						except:has = "NOT"
						if has == "OK":kk.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:kk.leaveGroup(receiver)
						try:kc.kickoutFromGroup(to, ["u1b227c131d7829e69956c06ff6db572c"]);has = "OK"
						except:has = "NOT"
						if has == "OK":kc.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:kc.leaveGroup(receiver)
						try:kd.kickoutFromGroup(to, ["udc7333bc03689e1eb494e4db5907e4f3"]);has = "OK"
						except:has = "NOT"
						if has == "OK":kd.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:kd.leaveGroup(receiver)
						try:ke.kickoutFromGroup(to, ["u2d0a791fd3294afac34446593332a74b"]);has = "OK"
						except:has = "NOT"
						if has == "OK":ke.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:ke.leaveGroup(receiver)
						try:a1.kickoutFromGroup(to, ["u734f29aae0e572a358d9e499ade73639"]);has = "OK"
						except:has = "NOT"
						if has == "OK":a1.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:a1.leaveGroup(receiver)
						try:a2.kickoutFromGroup(to, ["u8bb5a06bb4420b91b1b7d7a47450e26b"]);has = "OK"
						except:has = "NOT"
						if has == "OK":a2.leaveGroup(receiver)
						else:a2.leaveGroup(receiver)
						try:a3.kickoutFromGroup(to, ["u1eedd8a03bee09b3bd7df0a3b4bab51c"]);has = "OK"
						except:has = "NOT"
						if has == "OK":a3.sendReplyMessage(reply,receiver,"「 Normal ~ 」")
						else:a3.leaveGroup(receiver)
				if sentinel.startswith("cerberus:kick"):
					if sender in creator or sender in owner or sender in admin or sender in staff:
						key = eval(msg.contentMetadata["MENTION"])
						key["MENTIONEES"][0]["M"]
						targets = []
						for x in key["MENTIONEES"]:
							targets.append(x["M"])
						for target in targets:
							if target in Bots or target in creator or target in owner:
								try:
									nn = threading.Thread(target=kickprot, args=(receiver, sender)).start()
								except:
									pass
							else:
								try:
									haha = threading.Thread(target=blacklist, args=(target,)).start()
									huhu = threading.Thread(target=kickprot, args=(receiver, target)).start()
								except:
									klist = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
									for anu in klist:
										anu.sendReplyMessage(reply,receiver,"「 Limit -_- 」")
				if sentinel == "cerberus:reboot system":
					if sender in creator or sender in owner:
						cl.sendReplyMessage(reply,receiver,"「 Please Wait... 」")
						settings["restartPoint"] = receiver
						restartBot()
				if sentinel == "cerberus:blacklist user":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						if len(ban["blacklist"]) > 0:
							h = [a for a in ban["blacklist"]]
							k = len(h)//20
							for aa in range(k+1):
								if aa == 0:dd = '「 Blacklist User 」';no=aa
								else:dd = '';no=aa*20
								msgas = dd
								for a in h[aa*20:(aa+1)*20]:
									no+=1
									if no == len(h):msgas+='\n{}. @!'.format(no)
									else:msgas += '\n{}. @!'.format(no)
								sendMention(to, msgas, h[aa*20:(aa+1)*20])
						else:
							cl.sendReplyMessage(reply,receiver,"「 Doesn't Have Any Blacklist User -_- 」")
				if sentinel.startswith("cerberus:changepict:1"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][mid] = True
						cl.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						cl.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:2"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Amid] = True
						ki.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						ki.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:3"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Bmid] = True
						kk.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						kk.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:4"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Cmid] = True
						kc.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						kc.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:5"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Dmid] = True
						kd.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						kd.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:6"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Emid] = True
						ke.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						ke.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:7"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Fmid] = True
						a1.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						a1.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:8"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Gmid] = True
						a2.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						a2.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:9"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Hmid] = True
						a3.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						a3.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:ghost"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][Zmid] = True
						sw.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						sw.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changepict:all"):
					if sender in creator or sender in owner:
						settings["cerberusPict"][mid] = True
						settings["cerberusPict"][Amid] = True
						settings["cerberusPict"][Bmid] = True
						settings["cerberusPict"][Cmid] = True
						settings["cerberusPict"][Dmid] = True
						settings["cerberusPict"][Emid] = True
						settings["cerberusPict"][Fmid] = True
						settings["cerberusPict"][Gmid] = True
						settings["cerberusPict"][Hmid] = True
						settings["cerberusPict"][Zmid] = True
						u = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
						for a in u:
							a.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nPlease Send Picture You Want To Use")
					else:
						cl.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:1"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = cl.getProfile()
							dname.displayName = name
							cl.updateProfile(dname)
							cl.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						cl.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:2"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = ki.getProfile()
							dname.displayName = name
							ki.updateProfile(dname)
							ki.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						ki.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:3"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = kk.getProfile()
							dname.displayName = name
							kk.updateProfile(dname)
							kk.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						kk.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:4"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = kc.getProfile()
							dname.displayName = name
							kc.updateProfile(dname)
							kc.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						kc.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:5"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = kd.getProfile()
							dname.displayName = name
							kd.updateProfile(dname)
							kd.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						kd.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:6"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = ke.getProfile()
							dname.displayName = name
							ke.updateProfile(dname)
							ke.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						ke.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:7"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = a1.getProfile()
							dname.displayName = name
							a1.updateProfile(dname)
							a1.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						a1.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:8"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = a2.getProfile()
							dname.displayName = name
							a2.updateProfile(dname)
							a2.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						a2.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:9"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							dname = a3.getProfile()
							dname.displayName = name
							a3.updateProfile(dname)
							a3.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						a3.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:ghost"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							gname = sw.getProfile()
							gname.displayName = name
							sw.updateProfile(gname)
							sw.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
					else:
						sw.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changename:all"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							profile1 = cl.getProfile()
							profile1.displayName = name
							cl.updateProfile(profile1)
							cl.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile2 = ki.getProfile()
							profile2.displayName = name
							ki.updateProfile(profile2)
							ki.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile3 = kk.getProfile()
							profile3.displayName = name
							kk.updateProfile(profile3)
							kk.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile4 = kc.getProfile()
							profile4.displayName = name
							kc.updateProfile(profile4)
							kc.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile5 = kd.getProfile()
							profile5.displayName = name
							kd.updateProfile(profile5)
							kd.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile6 = ke.getProfile()
							profile6.displayName = name
							ke.updateProfile(profile6)
							ke.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile7 = a1.getProfile()
							profile7.displayName = name
							a1.updateProfile(profile7)
							a1.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile8 = a2.getProfile()
							profile8.displayName = name
							a2.updateProfile(profile8)
							a2.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							profile9 = a3.getProfile()
							profile9.displayName = name
							a3.updateProfile(profile9)
							a3.sendReplyMessage(reply,receiver,"「 Display Name 」\nChanged To {}".format(str(name)))
							ghost = sw.getProfile()
							ghost.displayName = name
							sw.updateProfile(ghost)
					else:
						a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
						for u in a:
							u.sendReplyMessage(reply,receiver,"「 Display Name 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:1"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = cl.getProfile()
							bio.statusMessage = name
							cl.updateProfile(bio)
							cl.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						cl.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:2"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = ki.getProfile()
							bio.statusMessage = name
							ki.updateProfile(bio)
							ki.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						ki.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:3"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = kk.getProfile()
							bio.statusMessage = name
							kk.updateProfile(bio)
							kk.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						kk.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("caroline:changebio:4"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = kc.getProfile()
							bio.statusMessage = name
							kc.updateProfile(bio)
							kc.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						kc.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:5"):
					if sender in creator or sendet in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = kd.getProfile()
							bio.statusMessage = name
							kd.updateProfile(bio)
							kd.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						kd.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:6"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = ke.getProfile()
							bio.statusMessage = name
							ke.updateProfile(bio)
							ke.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						ke.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:7"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = a1.getProfile()
							bio.statusMessage = name
							a1.updateProfile(bio)
							a1.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						a1.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:8"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = a2.getProfile()
							bio.statusMessage = name
							a2.updateProfile(bio)
							a2.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						a2.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:9"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio = a3.getProfile()
							bio.statusMessage = name
							a3.updateProfile(bio)
							a3.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						a3.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:ghost"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							ghost = sw.getProfile()
							ghost.statusMessage = name
							sw.updateProfile(ghost)
							sw.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
					else:
						sw.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel.startswith("cerberus:changebio:all"):
					if sender in creator or sender in owner:
						sep = text.split(" ")
						name = text.replace(sep[0] + " ","")
						if len(name) <= 99999999:
							bio1 = cl.getProfile()
							bio1.statusMessage = name
							cl.updateProfile(bio1)
							cl.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio2 = ki.getProfile()
							bio2.statusMessage = name
							ki.updateProfile(bio2)
							ki.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio3 = kk.getProfile()
							bio3.statusMessage = name
							kk.updateProfile(bio3)
							kk.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio4 = kc.getProfile()
							bio4.statusMessage = name
							kc.updateProfile(bio4)
							kc.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio5 = kd.getProfile()
							bio5.statusMessage = name
							kd.updateProfile(bio5)
							kd.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio6 = ke.getProfile()
							bio6.statusMessage = name
							ke.updateProfile(bio6)
							ke.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio7 = a1.getProfile()
							bio7.statusMessage = name
							a1.updateProfile(bio7)
							a1.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio8 = a2.getProfile()
							bio8.statusMessage = name
							a2.updateProfile(bio8)
							a2.sendReplyMessage(reply,receiver,"「 Status Message 」\nChanged To {}".format(str(name)))
							bio9 = a3.getProfile()
							bio9.statusMessage = name
							a3.updateProfile(bio9)
							ghost = sw.getProfile()
							ghost.statusMessage = name
							sw.updateProfile(ghost)
					else:
						a = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
						for u in a:
							u.sendReplyMessage(reply,receiver,"「 Status Message 」\nAccess Limited For Owner Only -_-")
				if sentinel == "cerberus:view bots":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						ma = ""
						a = 0
						for anu in Bots:
							a = a + 1
							end = '\n'
							ma += '┣ ' + str(a) + ". " +cl.getContact(anu).displayName + "\n"
						cl.sendReplyMessage(reply,receiver, "┏━ sᴇɴᴛɪɴᴇʟ™\n┣━━━━ List Bots\n"+ma+"┗━ Total「%s」Bots" %(str(len(Bots))))
				if sentinel == "cerberus:view grade":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						ma = ""
						mb = ""
						mc = ""
						md = ""
						a = 0
						b = 0
						c = 0
						d = 0
						for anu in creator:
							a = a + 1
							end = '\n'
							ma += '┣ ' + str(a) + ". " +cl.getContact(anu).displayName + "\n"
						for anu in owner:
							b = b + 1
							end = '\n'
							mb += '┣ ' + str(b) + ". " +cl.getContact(anu).displayName + "\n"
						for anu in admin:
							c = c + 1
							end = '\n'
							mc += '┣ ' + str(c) + ". " +cl.getContact(anu).displayName + "\n"
						for anu in staff:
							d = d + 1
							end = '\n'
							md += '┣ ' + str(d) + ". " +cl.getContact(anu).displayName + "\n"
						cl.sendReplyMessage(msg.id, to, "┏╸sᴇɴᴛɪɴᴇʟ™\n┣━━━━ List Access\n┣━━━━ Creator\n"+ma+"┣━━━━ Owner\n"+mb+"┣━━━━ Admin\n"+mc+"┣━━━━ Staff\n"+md+"┗━ Total「%s」Access" %(str(len(creator)+len(owner)+len(admin)+len(staff))))
				if sentinel == "cerberus:clearban":
					if sender in creator or sender in owner:
						if len(ban["blacklist"]) > 0:
							cl.sendReplyMessage(reply,receiver, "「 {} User Cleared 」".format(len(ban["blacklist"])))
							ban["blacklist"].clear()
						else:
							cl.sendReplyMessage(reply,receiver,"「 Doesn't Have Any Blacklist User -_- 」")
					else:
						cl.sendReplyMessage(reply,receiver,"「 Owner Permission -_- 」")
				if sentinel == "cerberus:byeall":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						bot = [cl,ki,kk,kc,kd,ke,a1,a2,a3]
						for hehe in bot:
							hehe.leaveGroup(receiver)
				if sentinel == "cerberus:1 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						cl.leaveGroup(receiver)
				if sentinel == "cerberus:2 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						ki.leaveGroup(receiver)
				if sentinel == "cerberus:3 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						kk.leaveGroup(receiver)
				if sentinel == "cerberus:4 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						kc.leaveGroup(receiver)
				if sentinel == "cerberus:5 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						kd.leaveGroup(receiver)
				if sentinel == "cerberus:6 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						ke.leaveGroup(receiver)
				if sentinel == "cerberus:7 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						a1.leaveGroup(receiver)
				if sentinel == "cerberus:8 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						a2.leaveGroup(receiver)
				if sentinel == "cerberus:9 @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						a3.leaveGroup(receiver)
				if sentinel == "cerberus:ghost @bye":
					if sender in creator or sender in owner or sender in admin or sender in staff:
						sw.leaveGroup(receiver)
		if msg.contentType == 13:
			if sender in creator:
				if settings["addowner"] == True:
					if msg.contentMetadata["mid"] in owner:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nContact Already In Owner Access -_-")
						settings["addowner"] = True
					else:
						status["owner"].append(msg.contentMetadata["mid"])
						settings["addowner"] = True
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nSuccess Add Contact To Owner Access ^_^")
				if settings["dellowner"] == True:
					if msg.contentMetadata["mid"] in owner:
						status["owner"].remove(msg.contentMetadata["mid"])
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nSuccess Delete Contact From Owner Access ^_^")
					else:
						settings["dellowner"] = True
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nContact Not In Owner Access -_-")
			if sender in creator or sender in owner:
				if settings["addadmin"] == True:
					if msg.contentMetadata["mid"] in admin:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nContact Already In Admin Access -_-")
						settings["addadmin"] = True
					else:
						status["admin"].append(msg.contentMetadata["mid"])
						settings["addadmin"] = True
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nSuccess Add Contact To Admin Access ^_^")
				if settings["delladmin"] == True:
					if msg.contentMetadata["mid"] in admin:
						status["admin"].remove(msg.contentMetadata["mid"])
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nSuccess Delete Contact From Admin Access ^_^")
					else:
						settings["delladmin"] = True
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nContact Not In Admin Access -_-")
			if sender in creator or sender in owner:
				if settings["addban"] == True:
					if msg.contentMetadata["mid"] in ban["blacklist"]:
						cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nContact Already In Blacklist -_-")
						settings["addban"] = True
					else:
						ban["blacklist"].append(msg.contentMetadata["mid"])
						settings["addban"] = True
						cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nSuccess Add Contact To Blacklist ^_^")
				if settings["dellban"] == True:
					if msg.contentMetadata["mid"] in ban["blacklist"]:
						ban["blacklist"].remove(msg.contentMetadata["mid"])
						cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nSuccess Delete Contact From Blacklist ^_^")
					else:
						settings["dellban"] = True
						cl.sendReplyMessage(reply,receiver,"「 Blacklist 」\nContact Not In Blacklist -_-")
			if sender in creator or sender in owner or sender in admin:
				if settings["addstaff"] == True:
					if msg.contentMetadata["mid"] in staff:
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nContact Already In Staff Access -_-")
						settings["addstaff"] = True
					else:
						settings["staff"].append(msg.contentMetadata["mid"])
						settings["addstaff"] = True
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nSuccess Add Contact To Staff Access ^_^")
				if settings["dellstaff"] == True:
					if msg.contentMetadata["mid"] in staff:
						settings["staff"].remove(msg.contentMetadata["mid"])
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nSuccess Delete Contact From Staff Access ^_^")
					else:
						settings["dellstaff"] = True
						cl.sendReplyMessage(reply,receiver,"「 Grant Access 」\nContact Not In Staff Access -_-")
			if sender in creator or sender in owner or sender in admin or sender in staff:
				if settings["addbots"] == True:
					if msg.contentMetadata["mid"] in Bots:
						cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nContact Already In Bot List -_-")
						settings["addbots"] = True
					else:
						settings["Bots"].append(msg.contentMetadata["mid"])
						settings["addbots"] = True
						cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nSuccess Add Contact To Bots List ^_^")
				if settings["dellbots"] == True:
					if msg.contentMetadata["mid"] in Bots:
						settings["Bots"].remove(msg.contentMetadata["mid"])
						cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nSuccess Delete Contact From Bots List ^_^")
					else:
						settings["dellbots"] = True
						cl.sendReplyMessage(reply,receiver,"「 Bots List 」\nContact Not In Bots List -_-")
		if msg.contentType == 1:
			if sender in creator or sender in owner:
				if mid in settings["cerberusPict"]:
					path = cl.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][mid]
					cl.updateProfilePicture(path)
					cl.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Amid in settings["cerberusPict"]:
					path = ki.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Amid]
					ki.updateProfilePicture(path)
					ki.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Bmid in settings["cerberusPict"]:
					path = kk.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Bmid]
					kk.updateProfilePicture(path)
					kk.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Cmid in settings["cerberusPict"]:
					path = kc.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Cmid]
					kc.updateProfilePicture(path)
					kc.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Dmid in settings["cerberusPict"]:
					path = kd.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Dmid]
					kd.updateProfilePicture(path)
					kd.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Emid in settings["cerberusPict"]:
					path = ke.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Emid]
					ke.updateProfilePicture(path)
					ke.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Fmid in settings["cerberusPict"]:
					path = a1.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Fmid]
					a1.updateProfilePicture(path)
					a1.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Gmid in settings["cerberusPict"]:
					path = a2.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Gmid]
					a2.updateProfilePicture(path)
					a2.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Hmid in settings["cerberusPict"]:
					path = a3.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Hmid]
					a3.updateProfilePicture(path)
					a3.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")
				if Zmid in settings["cerberusPict"]:
					path = sw.downloadObjectMsg(msg.id)
					del settings["cerberusPict"][Zmid]
					sw.updateProfilePicture(path)
					sw.sendReplyMessage(reply,receiver,"「 Profile Picture 」\nSuccess Change Profile Picture")

async def run():
	if settings["restartPoint"] is not None:
		res = "「 Bot Can Operate Again ^_^ 」"
		targets = cl.getGroupIdsJoined()
		for target in targets:
			try:
				cl.sendMessage(target, res)
			except TalkException:
				pass
			settings["restartPoint"] = None
	while 1:
		try:
			en = cl.poll.fetchOperations(cl.revision, 50)
			for op in en:
				if op.type != 0:
					cl.revision = max(cl.revision, op.revision)
					if op.type == 11:
						if settings["autoPurge"] == True:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel16 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
								except:
									pass
						if op.param1 in settings["protect"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									sntnel1 = threading.Thread(target=qrprot, args=(op.param1,)).start()
									sntnel2 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										sntnel3 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										sntnel4 = threading.Thread(target=qrprot, args=(op.param1,)).start()
										sntnel5 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									except:
										pass
						if op.param1 in settings["antijs"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel6 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
									sntnel7 = threading.Thread(target=qrprot, args=(op.param1,)).start()
									sntnel8 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									pass
						if op.param1 in settings["lockqr"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									wew = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									wew1 = threading.Thread(target=qrprot, args=(op.param1,)).start()
									wew2 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									pass
						if op.param1 in settings["warmode"]:
							if cl.getGroup(op.param1).preventedJoinByTicket == False:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
									pass
								else:
									wew3 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									try:
										wew4 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									except:
										try:
											wew5 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										except:
											try:
												settings["warmode"].remove(op.param1)
											except:
												pass
						if op.param2 in ban["blacklist"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									wew6 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									wew7 = threading.Thread(target=qrprot, args=(op.param1,)).start()
								except:
									pass
						if op.param3 in ban["blacklist"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									wew8 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									wew9 = threading.Thread(target=qrprot, args=(op.param1,)).start()
								except:
									pass
						if op.param3 == '1':
							if op.param1 in settings["lockname"]:
								try:
									G = cl.getGroup(op.param1)
								except:
									try:
										random.choice(KAC).getGroup(op.param1)
									except:
										try:
											random.choice(KAC).getGroup(op.param1)
										except:
											pass
								G.name = settings["lock_name"][op.param1]
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
									pass
								else:
									try:
										random.choice(KAC).updateGroup(G)
									except:
										try:
											random.choice(KAC).updateGroup(G)
										except:
											try:
												random.choice(KAC).updateGroup(G)
											except:
												pass
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
									pass
								else:
									try:
										wew10 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									except:
										try:
											wew11 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										except:
											try:
												wew12 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
											except:
												pass
												cl.sendMessage(op.param1,"Group Lock Name Activated")
												cl.sendMessage(op.param1,"Group Name Locked")
					if op.type == 13:
						if settings["autoPurge"] == True:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel17 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
								except:
									pass
						if op.param1 in settings["protect"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel9 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									sntnel10 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
									sntnel11 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									pass
						if op.param1 in settings["antijs"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel12 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
									sntnel13 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
									sntnel14 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									pass
						if op.param1 in settings["denyinvite"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									wew13 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
									wew14 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
								except:
									try:
										wew15 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
										wew16 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
									except:
										pass
						if op.param2 in ban["blacklist"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									wew17 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									wew18 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
									wew19 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										wew20 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
										wew21 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
										wew22 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									except:
										pass
						if op.param3 in ban["blacklist"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									wew23 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									wew24 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
									wew25 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										wew26 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
										wew27 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
										wew28 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									except:
										pass
						if mid in op.param3:
							if settings["autoLeave"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									cl.acceptGroupInvitation(op.param1)
								else:
									cl.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									cl.leaveGroup(op.param1)
						if mid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									cl.acceptGroupInvitation(op.param1)
								else:
									cl.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									cl.leaveGroup(op.param1)
						if Amid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									ki.acceptGroupInvitation(op.param1)
								else:
									ki.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									ki.leaveGroup(op.param1)
						if Bmid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									kk.acceptGroupInvitation(op.param1)
								else:
									kk.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									kk.leaveGroup(op.param1)
						if Cmid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									kc.acceptGroupInvitation(op.param1)
								else:
									kc.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									kc.leaveGroup(op.param1)
						if Dmid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									kd.acceptGroupInvitation(op.param1)
								else:
									kd.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									kd.leaveGroup(op.param1)
						if Emid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									ke.acceptGroupInvitation(op.param1)
								else:
									ke.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									ke.leaveGroup(op.param1)
						if Fmid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									a1.acceptGroupInvitation(op.param1)
								else:
									a1.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									a1.leaveGroup(op.param1)
						if Gmid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									a2.acceptGroupInvitation(op.param1)
								else:
									a2.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									a2.leaveGroup(op.param1)
						if Hmid in op.param3:
							if settings["autoJoin"] == True:
								if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in Bots:
									a3.acceptGroupInvitation(op.param1)
								else:
									a3.acceptGroupInvitation(op.param1)
									sendMention(op.param1,"Sorry @!,\nI Will Leave Because You Doesn't Have Access -_-",[op.param2])
									a3.leaveGroup(op.param1)
					if op.type == 17:
						if settings["autoPurge"] == True:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel18 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
								except:
									pass
						if op.param1 in settings["blockjoin"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									wew29 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									wew30 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									pass
						if op.param2 in ban["blacklist"]:
							try:
								wew31 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
							except:
								try:
									wew32 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
								except:
									pass
					if op.type == 19:
						if settings["autoPurge"] == True:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									sntnel19 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
								except:
									pass
						if op.param1 in settings["protect"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									uwew = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									uwew1 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										uwew2 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										uwew3 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									except:
										pass
						if op.param1 in settings["antijs"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									uwew4 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
									uwew5 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										uwew6 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									except:
										pass
						if op.param3 in mid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									uwew7 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									uwew8 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									uwew9 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									uwew10 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										uwew11 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										uwew12 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										uwew13 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										uwew14 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Amid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									uwew15 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									uwew16 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									uwew17 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									uwew18 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										uwew19 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										uwew20 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										uwew21 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										uwew22 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Bmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									uwew23 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									uwew24 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									uwew25 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									uwew26 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										uwew27 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										uwew28 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										uwew29 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										uwew30 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Cmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									uwew31 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									uwew32 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									rdwn = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									rdwn1 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										rdwn2 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										rdwn3 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										rdwn4 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										rdwn5 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Dmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									rdwn6 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									rdwn7 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									rdwn8 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									rdwn9 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										rdwn10 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										rdwn11 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										rdwn12 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										rdwn13 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Emid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									rdwn14 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									rdwn15 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									rdwn16 = threading.Thread(target=antijs3, args=(op.param1,)).start()
									rdwn17 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										rdwn18 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										rdwn19 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										rdwn20 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										rdwn21 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Fmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									rdwn22 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									rdwn23 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									rdwn24 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									rdwn25 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										rdwn26 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										rdwn27 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										rdwn28 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										rdwn29 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Gmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									rdwn30 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									rdwn31 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									rdwn32 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									var = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										var1 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										var2 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										var3 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										var4 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in Hmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var5 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var6 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									var7 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
									var8 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									try:
										var9 = threading.Thread(target=antijs3, args=(op.param1, op.param2)).start()
										var10 = threading.Thread(target=bckqrprot, args=(op.param1,)).start()
										var11 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										var12 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
									except:
										pass
						if op.param3 in creator:
							if op.param2 in Bots or op.param2 in cerberusbots:
								pass
							else:
								try:
									var13 = threading.Thread(target=kickprot, args=(op.param1, op.param3)).start()
									var14 = threading.Thread(target=inviteprot, args=(op.param1, op.param3)).start()
								except:
									try:
										G = random.choice(ABC).getGroup(op.param1)
										G.preventedJoinByTicket = False
										random.choice(ABC).updateGroup(G)
										Ti = random.choice(ABC).reissueGroupTicket(op.param1)
										sw.acceptGroupInvitationByTicket(op.param1,Ti)
										sw.kickoutFromGroup(op.param1, [op.param2])
										sw.findAndAddContactsByMid(op.param3)
										sw.inviteIntoGroup(op.param1, [op.param3])
										sw.leaveGroup(op.param1)
										var15 = threading.Thread(target=qrprot, args=(op.param1,)).start()
									except:
										pass
						if op.param3 in owner:
							if op.param2 in creator or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var16 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var17 = threading.Thread(target=inviteprot, args=(op.param1, op.param3)).start()
								except:
									try:
										G = random.choice(ABC).getGroup(op.param1)
										G.preventedJoinByTicket = False
										random.choice(ABC).updateGroup(G)
										Ti = random.choice(ABC).reissueGroupTicket(op.param1)
										sw.acceptGroupInvitationByTicket(op.param1,Ti)
										sw.kickoutFromGroup(op.param1, [op.param2])
										sw.findAndAddContactsByMid(op.param3)
										sw.inviteIntoGroup(op.param1, [op.param3])
										sw.leaveGroup(op.param1)
										var18 = threading.Thread(target=qrprot, args=(op.param1,)).start()
									except:
										pass
						if op.param3 in admin:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var19 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var20 = threading.Thread(target=inviteprot, args=(op.param1, op.param3)).start()
								except:
									try:
										G = random.choice(ABC).getGroup(op.param1)
										G.preventedJoinByTicket = False
										random.choice(ABC).updateGroup(G)
										Ti = random.choice(ABC).reissueGroupTicket(op.param1)
										sw.acceptGroupInvitationByTicket(op.param1,Ti)
										sw.kickoutFromGroup(op.param1, [op.param2])
										sw.findAndAddContactsByMid(op.param3)
										sw.inviteIntoGroup(op.param1, [op.param3])
										sw.leaveGroup(op.param1)
										var21 = threading.Thread(target=qrprot, args=(op.param1,)).start()
									except:
										pass
						if op.param3 in staff:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var22 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var23 = threading.Thread(target=inviteprot, args=(op.param1, op.param3)).start()
								except:
									try:
										G = random.choice(ABC).getGroup(op.param1)
										G.preventedJoinByTicket = False
										random.choice(ABC).updateGroup(G)
										Ti = random.choice(ABC).reissueGroupTicket(op.param1)
										sw.acceptGroupInvitationByTicket(op.param1,Ti)
										sw.kickoutFromGroup(op.param1, [op.param2])
										sw.findAndAddContactsByMid(op.param3)
										sw.inviteIntoGroup(op.param1, [op.param3])
										sw.leaveGroup(op.param1)
										var24 = threading.Thread(target=qrprot, args=(op.param1,)).start()
									except:
										pass
					if op.type == 32:
						if op.param1 in settings["antijs"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var25 = threading.Thread(target=antijs, args=(op.param1, op.param2)).start()
									var26 = threading.Thread(target=blacklist, args=(op.param2,)).start()
								except:
									pass
						if op.param1 in settings["protect"]:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								if op.param3 in ban["blacklist"]:
									try:
										var27 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
										var28 = threading.Thread(target=cancelprot, args=(op.param1, op.param3)).start()
										var29 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									except:
										pass
						if op.param3 == mid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var30 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var31 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var32 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Amid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var33 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var34 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var35 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Bmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var36 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var37 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var38 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Cmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var39 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var40 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var41 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Dmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var42 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var43 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var44 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Emid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var45 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var46 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var47 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Fmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var48 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var49 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var50 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Gmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var51 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var52 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var53 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
						if op.param3 == Hmid:
							if op.param2 in creator or op.param2 in owner or op.param2 in admin or op.param2 in staff or op.param2 in cerberusbots or op.param2 in Bots:
								pass
							else:
								try:
									var54 = threading.Thread(target=blacklist, args=(op.param2,)).start()
									var55 = threading.Thread(target=kickprot, args=(op.param1, op.param2)).start()
									var56 = threading.Thread(target=backupprot, args=(op.param1, op.param3)).start()
								except:
									pass
					if op.type == 26:
						RECEIVE_MESSAGE(op)
		except Exception as e:
			e = traceback.format_exc()
			if "EOFError" in e:
				pass
			elif "log_out" in e.lower():
				backupData()
				time.sleep(5)
				python = sys.executable
				os.execl(python, python, *sys.argv)
			elif "ShouldSyncException" in e:
				backupData()
				time.sleep(5)
				python3 = sys.executable
				os.execl(python3, python3, *sys.argv)
			elif "TalkException(code=8, reason='LOG_OUT', parameterMap=None)" in e:
				backupData()
				time.sleep(5)
				python = sys.executable
				os.execl(python, python, *sys.argv)
			elif "TalkException(code=20, reason='[UNCAUGHT_INTERNAL_ERROR] [UNCAUGHT_INTERNAL_ERROR] Login from secondary user blocked by userHash + clientType 8cb91561b450b38ccf0119fc4f5e37a3MA', parameterMap=None)" in e:
				backupData()
				time.sleep(5)
				python3 = sys.executable
				os.execl(python3, python3, *sys.argv)
			else:
				traceback.print_exc()
if __name__ == '__main__':
	print('####==== PROGRAM STARTED ====####')
	threading.Thread(target=event_loop.run_until_complete(run())).start()
