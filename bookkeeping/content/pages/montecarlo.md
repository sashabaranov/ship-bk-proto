Title: Monte-Carlo


<table class="table table-hover">
    <tr>
        <td><strong>Path</strong></td>
        <td><strong>Description</strong></td>
    </tr>


<!-- From Thomas -->
    <tr>
        <td><pre>
/eos/ship/data/pythia8_Geant4_total_Yandex2.root
/eos/ship/data/pythia8_Geant4_Yandex2_onlyNeutrinos.root
/eos/ship/data/pythia8_Geant4_total_Yandex.root
/eos/ship/data/pythia8_Geant4_Yandex_onlyMuons.root
/eos/ship/data/pythia8_Geant4_Yandex2_onlyMuons.root
/eos/ship/data/pythia8_Geant4_Yandex_onlyNeutrinos.root
        </pre>
        </td>
        <td>MCParticles after hadron absorber, energy cut used E>10GeV.</td>
    </tr>


    <tr>
        <td><pre>
/eos/ship/data/pythia8_Geant4_onlyMuons.root
/eos/ship/data/pythia8_Geant4_onlyNeutrinos.root
/eos/ship/data/pythia8_Geant4_total.root
        </pre>
        </td>
        <td>MCParticles after hadron absorber, mixture of energy cuts used: E>1,5,10 and 100 GeV.</td>
    </tr>




<!-- From Nathalie -->



<!--
List and description of files on EOS (for nu-BG):
General Information:
How is the Data generated - steps:
1.) Generate events in GENIE
2.) process with script run_simScript.py (from FAIRSHIP) => raw ntuple
3.) reconstruct events with ShipReco.py (from FAIRSHIP) => reconstructed ntuple
4.) get interesting numbers with ntuple_nuVeto*.py  => Final ntuple/output ntuple

What files were used in TP:
nu:      /eos/ship/data/neutrinoBackground/Yandex_for_TP/newGen_11560000_nuBg_total.root
antinu:  /eos/ship/data/neutrinoBackground/Yandex_for_TP/antinu_full.10.0.Genie-TGeant4.root

What files were used for Addendum:
nu:      /eos/ship/data/nuDataTP-DOCA-Repro/
       + /eos/ship/data/nuDataAdditionalProduction/

antinu:  /eos/ship/data/antinuDataTP-DOCA-Repro/output-DOCA-Repro-antinu-1670000-addWeight_100mradcut.root
       + /eos/ship/data/antinuAdditionalProduction/outputAugustAdditional-antinu-20000000.root

-->

<!-- Antinu -->

    <tr>
        <td><pre>
/eos/ship/data/antinuAdditionalProduction/
        </pre>
        </td>
        <td>Is the folder with the files for the additional antinu Production for the Addendum.
This events were generated to increase the statistic in all the bins.
The energy range goes from 2 GeV to 200 GeV. (nu only goes up to 100 GeV).
As inputspektrum was the Histogram used from Prof. G. De Lellis with an applied 100mrad cut.
The folders inside are 'output' and 'rec'. The 'output' contains the final ntuple used in the Addendum 
and the 'rec' folder contains the files after the FAIRSHIP Reconstruction (using ShipReco.py) (version in August 2015)
</td>
    </tr>

    <tr>
        <td><pre>
/eos/ship/data/antinuDataTP/
        </pre>
        </td>
        <td>
        Contains the 'RAW' and 'REC' Data. 'RAw' is the ntuple before applying a reconstruction and 'REC' is after applying the reconstruction.
        Here the reconstruction used was the same as for the TP (reconstruction version in March 2015)
        </td>
    </tr>


        <td><pre>
/eos/ship/data/antinuDataTP-DOCA-Repro/
        </pre>
        </td>
        <td>
        Contains the final ntuple (output ntuple) used for the Addendum. 
        As input the files in /eos/ship/data/antinuDataTP/antinu_raw.tar were used and the reconstruction
        version in August was used. As input spectrum Hans energy spectrum was used. To adjust to G. De Lellis spectrum
        an additional version was produced: output-DOCA-Repro-antinu-1670000-addWeight_100mradcut.root
        This one was then combined with outputAugustAdditional-antinu-20000000.root for the Addendum
        </td>
    </tr>


<!-- Nu -->



<tr>
<td><pre>/eos/ship/data/nuDataAdditionalProduction/</pre></td>
<td>Is the folder with the files for the additional nu Production for the Addendum.
This events were generated to increase the statistic in the first and second bins.
The energy range goes from 2 GeV to 10 GeV.
As inputspektrum was the Histogram used from Prof. G. De Lellis with an applied 100mrad cut.
The folders inside are 'output' and 'rec'. The 'output' contains the final ntuple used in the Addendum
and the 'rec' folder contains the files after the FAIRSHIP Reconstruction (using ShipReco.py) (version in August 2015)</td>
</tr>

<tr>
<td><pre>/eos/ship/data/nuDataTP/</pre></td>
<td>Contains all the reconstructed files that where later used for the TP.</td>
</tr>

<tr>
<td><pre>/eos/ship/data/nuDataTP_raw/</pre></td>
<td>Contains the 'RAw' ntuple before applying a reconstruction. Used for the TP and as input for the Addendum ntuple.</td>
</tr>

<tr>
<td><pre>/eos/ship/data/nuDataTP-DOCA-Repro/</pre></td>
<td>Contains the final ntuple (output ntuple) used for the Addendum. 
As input the files in /eos/ship/data/nuDataTP_raw/ were used and the reconstruction
version in August was used. As input spectrum Hans energy spectrum was used. To adjust to G. De Lellis spectrum
an additional version was produced: output-DOCA-Repro-nu-15530000-addWeight_100mradcut.root
This one was then combined with outputAugustAdditional-energy2-10-nu-10000000.root for the Addendum</td>
</tr>


<tr>
<td><pre>/eos/ship/data/antinuDataReprocessingAugust2015/</pre></td>
<td>Contains all antinu output files (final ntuple for analysis) after taking the reconstructed data from the TP and applying the 
same last step (ntuple_nuVeto_small_newVar.py). IS MISSING THE NoB_DOCA LEAF - it's filled with 0.
NOT USED FOR ADDENDUM
</td>
</tr>

<tr>
<td><pre>/eos/ship/data/nuDataReprocessingAugust2015/</pre></td>
<td>Contains all nu output files (final ntuple for analysis) after taking the reconstructed data from the TP and applying the 
same last step (ntuple_nuVeto_small_newVar.py). IS MISSING THE NoB_DOCA LEAF - it's filled with 0.
NOT USED FOR ADDENDUM
</td>
</tr>

<tr>
<td><pre>/eos/ship/data/nu-antinu-ntuples/</pre></td>
<td>Contains the ntuples after a reprocessing (recontruction + ntuple_nuVeto_small_newVar.py) in June 2015
As input spectrum Hans spectrum was used.
NOT USED FOR ADDENDUM
</td>
</tr>







</table>
