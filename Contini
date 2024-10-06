% file name = Contini
% date of creation = 23/05/2023
%
close all
clear all
%
%-------------------------------------------------------------------------------
% US population
%-------------------------------------------------------------------------------
%
height(1) = 161.3; % height of female (cm)
height(2) = 175.3; % height of male (cm)
width1 = [0.245*height(1),0.259*height(2)]; % from the tip of one clavicole to the tip of the other
width2 = [0.219*height(1),0.200*height(2)]; % from one head of one femur to the head of the other
width3 = [0.057*height(1),0.055*height(2)]; % width of the footh
Length1 = [0.938*height(1),0.936*height(2)];
Length2 = [0.875*height(1),0.870*height(2)];
Length3 = [0.825*height(1),0.819*height(2)];
Length4 = [0.632*height(1),0.630*height(2)];
Length5 = [0.480*height(1),0.485*height(2)];
Length6 = [0.370*height(1),0.357*height(2)];
Length7 = [0.524*height(1),0.530*height(2)];
Length8 = [0.282*height(1),0.285*height(2)];
Length9 = [0.048*height(1),0.043*height(2)];
js = 5 % joint size
shift = [0,100] % I use this to shift the second plot on the right
%
figure(1)
%
for (i=1:2)
  %
  H = height(i)
  w1 = width1(i)
  w2 = width2(i)
  w3 = width3(i)
  L1 = Length1(i)
  L2 = Length2(i)
  L3 = Length3(i)
  L4 = Length4(i)
  L5 = Length5(i)
  L6 = Length6(i)
  L7 = Length7(i)
  L8 = Length8(i)
  L9 = Length9(i)
  h = H - L2 % head height
  l = h/3 % head width divided by two
  %
  %-------------------------------------------------------------------------------
  % bones
  %-------------------------------------------------------------------------------
  %
  plot([0+shift(i),0+shift(i)],[H-h,L7],"-k","linewidth",1.5) % backbone
  hold on
  rectangle ("Position",[-l+shift(i),H-h,2*l,h],"linewidth",1.5) % head
  plot([-l+shift(i),l+shift(i)],[L1,L1],"-k","linewidth",1.5) % eyes
  %
  plot([-w1/2+shift(i),w1/2+shift(i)],[L3,L3],"-k","linewidth",1.5) % shoulders (tips of the clavicles)
  %
  plot([-w1/2+shift(i),-w1/2+shift(i)],[L3,L4],"-k","linewidth",1.5) % homerus, left
  plot([w1/2+shift(i),w1/2+shift(i)],[L3,L4],"-k","linewidth",1.5) % homerus, rigth
  %
  plot([-w1/2+shift(i),-w1/2+shift(i)],[L4,L5],"-k","linewidth",1.5) % radius, left
  plot([w1/2+shift(i),w1/2+shift(i)],[L4,L5],"-k","linewidth",1.5) % radius, rigth
  %
  rectangle ("Position",[-w1/2-(3/4)*l/2+shift(i),L6,(3/4)*l,L5-L6],"linewidth",1.5) % hand, left
  rectangle ("Position",[w1/2-(3/4)*l/2+shift(i),L6,(3/4)*l,L5-L6],"linewidth",1.5) % hand, rigth
  %
  plot([-w2/2+shift(i),w2/2+shift(i)],[L7,L7],"-k","linewidth",1.5) % hip
  %
  plot([-w3+shift(i),w3+shift(i)],[0,0],"-k","linewidth",1.5) % feet, plant
  %
  plot([-w3+shift(i),-w3/2+shift(i)],[0,L9],"-k","linewidth",1.5) % ankle, left
  plot([-w3/2+shift(i),0+shift(i)],[L9,0],"-k","linewidth",1.5) % ankle, left
  plot([0+shift(i),w3/2+shift(i)],[0,L9],"-k","linewidth",1.5) % ankle, rigth
  plot([w3/2+shift(i),w3+shift(i)],[L9,0],"-k","linewidth",1.5) % ankle, rigth
  %
  plot([-w3/2+shift(i),-w3+shift(i)],[L9,L8],"-k","linewidth",1.5) % tibia, left
  plot([w3/2+shift(i),w3+shift(i)],[L9,L8],"-k","linewidth",1.5) % tibia, rigth
  %
  plot([-w2/2+shift(i),-w3+shift(i)],[L7,L8],"-k","linewidth",1.5) % femur, left
  plot([w2/2+shift(i),w3+shift(i)],[L7,L8],"-k","linewidth",1.5) % femur, rigth
  %
  %-------------------------------------------------------------------------------
  % joints
  %-------------------------------------------------------------------------------
  %
  plot(-w1/2+shift(i),L3,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % shoulder, left
  plot(w1/2+shift(i),L3,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % shoulder, rigth
  %
  plot(-w1/2+shift(i),L4,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % elbow, left
  plot(w1/2+shift(i),L4,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % elbow, rigth
  %
  plot(-w1/2+shift(i),L5,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % wirst, left
  plot(w1/2+shift(i),L5,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % wirst, rigth
  %
  plot(-w2/2+shift(i),L7,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % hip, left
  plot(w2/2+shift(i),L7,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % hip, rigth
  %
  plot(-w3+shift(i),L8,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % knee, left
  plot(w3+shift(i),L8,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % knee, rigth
  %
  plot(-w3/2+shift(i),L9,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % ankle, left
  plot(w3/2+shift(i),L9,'o','markersize',js,'markerfacecolor','k','markeredgecolor','k') % ankle, rigth
  %
  %-------------------------------------------------------------------------------
  % measures
  %-------------------------------------------------------------------------------
  %
  L = H/3;
  % head
  plot([-L+shift(i),0+shift(i)],[H,H],"--k","linewidth",1.0)
  plot([-L+shift(i),0+shift(i)],[H-h,H-h],"--k","linewidth",1.0)
  quiver(-L+shift(i),H-h,0,h,'-k',"maxheadsize",0.1)
  quiver(-L+shift(i),H,0,-h,'-k',"maxheadsize",0.1)
  factorH = h/H;
  text (-L+l/2+shift(i),H-h/2,strcat("h=",num2str(factorH),"H"),"fontsize",15)
  % homer
  homer = L3 - L4;
  plot([-L+shift(i),-w1/2+shift(i)],[L3,L3],"--k","linewidth",1.0)
  plot([-L+shift(i),-w1/2+shift(i)],[L4,L4],"--k","linewidth",1.0)
  quiver(-L+shift(i),L4,0,homer,'-k',"maxheadsize",0.1)
  quiver(-L+shift(i),L3,0,-homer,'-k',"maxheadsize",0.1)
  factorH = homer/H;
  factorh = homer/h;
  text (-L+l/2+shift(i),L3-homer/2,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15)
  % radius
  radius = L4 - L5;
  plot([-L+shift(i),-w1/2+shift(i)],[L4,L4],"--k","linewidth",1.0)
  plot([-L+shift(i),-w1/2+shift(i)],[L5,L5],"--k","linewidth",1.0)
  quiver(-L+shift(i),L5,0,radius,'-k',"maxheadsize",0.1)
  quiver(-L+shift(i),L4,0,-radius,'-k',"maxheadsize",0.1)
  factorH = radius/H;
  factorh = radius/h;
  text (-L+l/2+shift(i),L4-radius/2,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15)
  % hand
  hand = L5 - L6;
  plot([-L+shift(i),-w1/2+shift(i)],[L5,L5],"--k","linewidth",1.0)
  plot([-L+shift(i),-w1/2+shift(i)],[L6,L6],"--k","linewidth",1.0)
  quiver(-L+shift(i),L6,0,hand,'-k',"maxheadsize",0.1)
  quiver(-L+shift(i),L5,0,-hand,'-k',"maxheadsize",0.1)
  factorH = hand/H;
  factorh = hand/h;
  text (-L+l/2+shift(i),L5-hand/2,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15)
  % femur
  femur = L7 - L8;
  plot([-1.1*L+shift(i),-w1/2+shift(i)],[L7,L7],"--k","linewidth",1.0)
  plot([-1.1*L+shift(i),-w3+shift(i)],[L8,L8],"--k","linewidth",1.0)
  quiver(-1.1*L+shift(i),L8,0,femur,'-k',"maxheadsize",0.1)
  quiver(-1.1*L+shift(i),L7,0,-femur,'-k',"maxheadsize",0.1)
  factorH = femur/H;
  factorh = femur/h;
  text (-1.1*L+l/2+shift(i),L7-homer,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15)
  % tibia
  tibia = L8 - L9;
  plot([-L+shift(i),-w3+shift(i)],[L8,L8],"--k","linewidth",1.0)
  plot([-L+shift(i),-w3/2+shift(i)],[L9,L9],"--k","linewidth",1.0)
  quiver(-L+shift(i),L8,0,-tibia,'-k',"maxheadsize",0.1)
  quiver(-L+shift(i),L9,0,tibia,'-k',"maxheadsize",0.1)
  factorH = tibia/H;
  factorh = tibia/h;
  text (-L+l/2+shift(i),L8-tibia/2,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15)
  % ankle
  ankle = L9;
  plot([-L+shift(i),-w3/2+shift(i)],[0,0],"--k","linewidth",1.0)
  quiver(-L+shift(i),L9,0,-ankle,'-k',"maxheadsize",0.1)
  quiver(-L+shift(i),0,0,ankle,'-k',"maxheadsize",0.1)
  factorH = ankle/H;
  factorh = ankle/h;
  text (-L+l/2+shift(i),L9-ankle/2,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15)
  % shoulders
  quiver(-w1/2+shift(i),L3-l,w1/2,0,'-k',"maxheadsize",0.1)
  quiver(0+shift(i),L3-l,-w1/2,0,'-k',"maxheadsize",0.1)
  factorH = w1/(2*H);
  factorh = w1/(2*h);
  text (-2*l+shift(i),L3-2*l,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15,"backgroundcolor","white")
  % hips
  plot([-w2/2+shift(i),-w2/2+shift(i)],[L7,L7+2*l],"--k","linewidth",1.0)
  quiver(-w2/2+shift(i),L4-l,w2/2,0,'-k',"maxheadsize",0.1)
  quiver(0+shift(i),L4-l,-w2/2,0,'-k',"maxheadsize",0.1)
  factorH = w2/(2*H);
  factorh = w2/(2*h);
  text (-2*l+shift(i),L4-1.7*l,strcat(num2str(factorH),"H=",strcat(num2str(factorh),"h")),"fontsize",15,"backgroundcolor","white")
  % heads
  plot([w2/2+1.5*l+shift(i),w2/2+1.5*l+shift(i)],[H,0],"-k","linewidth",1.0)
  temp=0;
  while (temp<=H)
    plot(w2/2+1.5*l+shift(i),H-temp,'^','markersize',js,'markerfacecolor','k','markeredgecolor','k')
    temp=temp+h;
  endwhile
endfor
%
%-------------------------------------------------------------------------------
% grid and axes
%-------------------------------------------------------------------------------
%
axis([-70,140,-l,H+l],"equal")
ylabel("cm","fontsize",15)
grid on
grid minor
